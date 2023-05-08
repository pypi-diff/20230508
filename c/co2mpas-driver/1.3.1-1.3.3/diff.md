# Comparing `tmp/co2mpas_driver-1.3.1.tar.gz` & `tmp/co2mpas_driver-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co2mpas_driver-1.3.1.tar", last modified: Fri Oct 14 10:51:28 2022, max compression
+gzip compressed data, was "co2mpas_driver-1.3.3.tar", last modified: Mon May  8 12:10:23 2023, max compression
```

## Comparing `co2mpas_driver-1.3.1.tar` & `co2mpas_driver-1.3.3.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.227707 co2mpas_driver-1.3.1/
--rw-rw-rw-   0        0        0     1096 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/AUTHORS.rst
--rw-rw-rw-   0        0        0    13407 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0    11915 2022-10-14 10:51:28.227707 co2mpas_driver-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    10691 2022-10-14 10:46:52.000000 co2mpas_driver-1.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.164085 co2mpas_driver-1.3.1/co2mpas_driver/
--rw-rw-rw-   0        0        0     2142 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/README.md
--rw-rw-rw-   0        0        0     1903 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/__init__.py
--rw-rw-rw-   0        0        0      106 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/_version.py
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.202500 co2mpas_driver-1.3.1/co2mpas_driver/common/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/__init__.py
--rw-rw-rw-   0        0        0    21259 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/defaults.py
--rw-rw-rw-   0        0        0    13624 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/functions.py
--rw-rw-rw-   0        0        0     5342 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/gear_functions.py
--rw-rw-rw-   0        0        0     3380 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/generic_co2mpas.py
--rw-rw-rw-   0        0        0     1028 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/plot_templates.py
--rw-rw-rw-   0        0        0     1870 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/reading_n_organizing.py
--rw-rw-rw-   0        0        0     1502 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/simulation_part.py
--rw-rw-rw-   0        0        0     9315 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/utils.py
--rw-rw-rw-   0        0        0    14718 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/vehicle_functions.py
--rw-rw-rw-   0        0        0     7607 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/common/vehicle_specs_class.py
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.204743 co2mpas_driver-1.3.1/co2mpas_driver/db/
--rw-rw-rw-   0        0        0    60717 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/db/EuroSegmentCar.csv
--rw-rw-rw-   0        0        0    39924 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/db/EuroSegmentCar_cleaned.csv
--rw-rw-rw-   0        0        0      790 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/euro_segment.py
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.215358 co2mpas_driver-1.3.1/co2mpas_driver/examples/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/Sim_Kat_for_Jaime_2.py
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/new_test.py
--rw-rw-rw-   0        0        0     5178 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py
--rw-rw-rw-   0        0        0     2896 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_gear_shifting.py
--rw-rw-rw-   0        0        0     3398 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_light_co2mpas.py
--rw-rw-rw-   0        0        0     3961 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_simulation.py
--rw-rw-rw-   0        0        0     8119 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_varying_des_speed.py
--rw-rw-rw-   0        0        0     2976 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_veh_specs_collection.py
--rw-rw-rw-   0        0        0     2302 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/examples/test.py
--rw-rw-rw-   0        0        0     7145 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/load.py
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.220631 co2mpas_driver-1.3.1/co2mpas_driver/model/
--rw-rw-rw-   0        0        0    34477 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/model/__init__.py
--rw-rw-rw-   0        0        0     7881 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/model/co2mpas.py
--rw-rw-rw-   0        0        0     8210 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/model/driver.py
--rw-rw-rw-   0        0        0     3502 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/model/simulation.py
--rw-rw-rw-   0        0        0     3361 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/plot.py
--rw-rw-rw-   0        0        0     2745 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/sample_simulation.py
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.221647 co2mpas_driver-1.3.1/co2mpas_driver/template/
--rw-rw-rw-   0        0        0    15512 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/co2mpas_driver/template/sample.xlsx
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.190211 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/
--rw-rw-rw-   0        0        0    11915 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1750 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-14 10:51:28.000000 co2mpas_driver-1.3.1/co2mpas_driver.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2022-10-14 10:51:28.225684 co2mpas_driver-1.3.1/model_validation/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/model_validation/__init__.py
--rw-rw-rw-   0        0        0      996 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/model_validation/test_core.py
--rw-rw-rw-   0        0        0     5497 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/model_validation/test_model.py
--rw-rw-rw-   0        0        0     1123 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.1/model_validation/utils.py
--rw-rw-rw-   0        0        0       42 2022-10-14 10:51:28.227707 co2mpas_driver-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3015 2022-10-14 10:49:44.000000 co2mpas_driver-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.220894 co2mpas_driver-1.3.3/
+-rw-rw-rw-   0        0        0     1096 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0    13407 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    11983 2023-05-08 12:10:23.220390 co2mpas_driver-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10795 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.157581 co2mpas_driver-1.3.3/co2mpas_driver/
+-rw-rw-rw-   0        0        0     2142 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/README.md
+-rw-rw-rw-   0        0        0     1903 2023-05-08 08:07:10.000000 co2mpas_driver-1.3.3/co2mpas_driver/__init__.py
+-rw-rw-rw-   0        0        0      104 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.189455 co2mpas_driver-1.3.3/co2mpas_driver/common/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/__init__.py
+-rw-rw-rw-   0        0        0    21259 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/defaults.py
+-rw-rw-rw-   0        0        0    13600 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/functions.py
+-rw-rw-rw-   0        0        0     5342 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/gear_functions.py
+-rw-rw-rw-   0        0        0     3436 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/generic_co2mpas.py
+-rw-rw-rw-   0        0        0     1028 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/plot_templates.py
+-rw-rw-rw-   0        0        0     1870 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/reading_n_organizing.py
+-rw-rw-rw-   0        0        0     1500 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/simulation_part.py
+-rw-rw-rw-   0        0        0     9313 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/utils.py
+-rw-rw-rw-   0        0        0    14718 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_functions.py
+-rw-rw-rw-   0        0        0     7883 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_specs_class.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.193231 co2mpas_driver-1.3.3/co2mpas_driver/db/
+-rw-rw-rw-   0        0        0    60717 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar.csv
+-rw-rw-rw-   0        0        0    42723 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned.csv
+-rw-rw-rw-   0        0        0    42723 2023-04-10 21:50:10.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv
+-rw-rw-rw-   0        0        0      790 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/euro_segment.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.207205 co2mpas_driver-1.3.3/co2mpas_driver/examples/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/Sim_Kat_for_Jaime_2.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/__init__.py
+-rw-rw-rw-   0        0        0     1212 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/calculate_on_existing_example.py
+-rw-rw-rw-   0        0        0     9263 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/mfc_post_proc_trajectory.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/new_test.py
+-rw-rw-rw-   0        0        0     5178 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py
+-rw-rw-rw-   0        0        0     2896 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_gear_shifting.py
+-rw-rw-rw-   0        0        0     3398 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_light_co2mpas.py
+-rw-rw-rw-   0        0        0     3961 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_simulation.py
+-rw-rw-rw-   0        0        0     8119 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed.py
+-rw-rw-rw-   0        0        0    11012 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed_yl_2.py
+-rw-rw-rw-   0        0        0     2976 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_veh_specs_collection.py
+-rw-rw-rw-   0        0        0     2302 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/test.py
+-rw-rw-rw-   0        0        0     7770 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/load.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.212869 co2mpas_driver-1.3.3/co2mpas_driver/model/
+-rw-rw-rw-   0        0        0    41159 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/__init__.py
+-rw-rw-rw-   0        0        0     8227 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/co2mpas.py
+-rw-rw-rw-   0        0        0    16433 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/driver.py
+-rw-rw-rw-   0        0        0     4983 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/simulation.py
+-rw-rw-rw-   0        0        0     3361 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/plot.py
+-rw-rw-rw-   0        0        0     2745 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/sample_simulation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.213869 co2mpas_driver-1.3.3/co2mpas_driver/template/
+-rw-rw-rw-   0        0        0    15512 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/template/sample.xlsx
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.177758 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/
+-rw-rw-rw-   0        0        0    11983 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1964 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.217870 co2mpas_driver-1.3.3/model_validation/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/__init__.py
+-rw-rw-rw-   0        0        0      996 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/test_core.py
+-rw-rw-rw-   0        0        0     5659 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/model_validation/test_model.py
+-rw-rw-rw-   0        0        0     1123 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:10:23.220894 co2mpas_driver-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     3037 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/setup.py
```

### Comparing `co2mpas_driver-1.3.1/AUTHORS.rst` & `co2mpas_driver-1.3.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/LICENSE.txt` & `co2mpas_driver-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/PKG-INFO` & `co2mpas_driver-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: co2mpas_driver
-Version: 1.3.1
+Version: 1.3.3
 Summary: A lightweight microsimulation free-flow acceleration model(MFC) or co2mpas_driver is a model that is able to capture the vehicle acceleration dynamics accurately and consistently
 License: European Union Public Licence 1.1 or later (EUPL 1.1+)
-Project-URL: Sources, https://github.com/JRCSTU/co2mpas_driver
+Project-URL: Sources, https://code.europa.eu/jrc-ldv/co2mpas_driver
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -16,22 +16,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
-.. figure:: ./co2mpas_driver/images/co2mpas_driver_logo.png
-    :align: center
-    :alt: alternate text
-    :figclass: align-center
+|JRC-image|
 
 .. _start-info:
 
 
 :versions:      |gh-version| |rel-date| |python-ver|
 :documentation: https://co2mpas-driver.readthedocs.io/en/latest/
 :sources:       https://code.europa.eu/jrc-ldv/co2mpas-driver |pypi-ins| |codestyle|
@@ -129,16 +125,17 @@
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
 
 * *co2mpas_driver* must be imported as a dispatcher (dsp). The dsp contains
   functions to process vehicle data and run the *com2pas_driver* model. Also is necessary
   to import *schedula* for selecting and executing functions from the *co2mpas_driver*.
   For more information on how to use *schedula*: https://pypi.org/project/schedula/
-      >>> from co2mpas_driver import dsp
-      >>> import schedula as sh
+  
+        >>> from co2mpas_driver import dsp
+        >>> import schedula as sh
 
 Load data
 ---------
 * Load vehicle data for a specific vehicle from vehicles database
 
         >>> db_path = 'EuroSegmentCar.csv'
 
@@ -281,19 +278,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitHub%20-1.3.1-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2022/10/14-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -307,14 +304,19 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.0-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
+.. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
+    :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
+    :alt: GitLab repository
+
+
 .. |CO2| replace:: CO\ :sub:`2`
 
 .. _end-sub:
```

### Comparing `co2mpas_driver-1.3.1/README.rst` & `co2mpas_driver-1.3.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-.. figure:: ./co2mpas_driver/images/co2mpas_driver_logo.png
-    :align: center
-    :alt: alternate text
-    :figclass: align-center
+|JRC-image|
 
 .. _start-info:
 
 
 :versions:      |gh-version| |rel-date| |python-ver|
 :documentation: https://co2mpas-driver.readthedocs.io/en/latest/
 :sources:       https://code.europa.eu/jrc-ldv/co2mpas-driver |pypi-ins| |codestyle|
@@ -103,16 +100,17 @@
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
 
 * *co2mpas_driver* must be imported as a dispatcher (dsp). The dsp contains
   functions to process vehicle data and run the *com2pas_driver* model. Also is necessary
   to import *schedula* for selecting and executing functions from the *co2mpas_driver*.
   For more information on how to use *schedula*: https://pypi.org/project/schedula/
-      >>> from co2mpas_driver import dsp
-      >>> import schedula as sh
+  
+        >>> from co2mpas_driver import dsp
+        >>> import schedula as sh
 
 Load data
 ---------
 * Load vehicle data for a specific vehicle from vehicles database
 
         >>> db_path = 'EuroSegmentCar.csv'
 
@@ -255,19 +253,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitHub%20-1.3.1-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2022/10/14-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -281,14 +279,19 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.0-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
+.. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
+    :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
+    :alt: GitLab repository
+
+
 .. |CO2| replace:: CO\ :sub:`2`
 
 .. _end-sub:
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/README.md` & `co2mpas_driver-1.3.3/co2mpas_driver/README.md`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/__init__.py` & `co2mpas_driver-1.3.3/co2mpas_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/defaults.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/defaults.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/functions.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import math
-import numpy
+import numpy as np
 
 
 def calculate_wheel_power(velocities, acc, road_loads, veh_mass, slope):
     """
     Calculates the wheel power [kW].
 
     :param velocities:
-        Velocity [km/h].
+        Velocity [m/s].
     :type velocities: numpy.array | float
 
     :param acc:
         Acceleration [m/s2].
     :type acc: numpy.array | float
 
     :param road_loads:
@@ -32,26 +32,24 @@
 
     ;param slope:
         Slope in tangent
     """
 
     f0, f1, f2 = road_loads
 
-    # quadratic_term = f0 * math.cos(math.atan(slope)) + (f1 + f2 * velocities) * velocities
-    #
-    # vel = velocities / 3600
+    velocities_km_h = velocities * 3.6
 
     quadratic_term = (
         f0 * math.cos(math.atan(slope))
-        + (f1 + f2 * velocities) * velocities
+        + (f1 + f2 * velocities_km_h) * velocities_km_h
         + 1.03 * veh_mass * acc
         + veh_mass * math.sin(math.atan(slope)) * 9.81
     )
 
-    res = float(quadratic_term * velocities) / 3600
+    res = float(quadratic_term * velocities) / 1000
 
     return res
 
 
 def calculate_min_wheel_torque(
     velocities, accelerations, road_loads, vehicle_mass, f, r_dynamic
 ):
@@ -101,27 +99,27 @@
 
 
 def calculate_wheel_speeds(velocities, r_dynamic):
     """
     Calculates rotating speed of the wheels [RPM].
 
     :param velocities:
-        Vehicle velocity [km/h].
+        Vehicle velocity [m/s].
     :type velocities: numpy.array | float
 
     :param r_dynamic:
         Dynamic radius of the wheels [m].
     :type r_dynamic: float
 
     :return:
         Rotating speed of the wheel [RPM].
     :rtype: numpy.array | float
     """
 
-    return velocities * (30.0 / (3.6 * math.pi * r_dynamic))
+    return velocities * 30.0 / (math.pi * r_dynamic)
 
 
 def calculate_wheel_torques(wheel_powers, wheel_speeds):
     """
     Calculates torque at the wheels [N*m].
 
     :param wheel_powers:
@@ -134,16 +132,16 @@
 
     :return:
         Torque at the wheels [N*m].
     :rtype: numpy.array | float
     """
 
     pi = math.pi
-    if isinstance(wheel_speeds, numpy.ndarray):
-        return numpy.nan_to_num(wheel_powers / wheel_speeds * (30000.0 / pi))
+    if isinstance(wheel_speeds, np.ndarray):
+        return np.nan_to_num(wheel_powers / wheel_speeds * (30000.0 / pi))
     return wheel_powers / wheel_speeds * (30000.0 / pi) if wheel_speeds else 0.0
 
 
 def calculate_final_drive_speeds_in(final_drive_speeds_out, final_drive_ratio_vector):
     """
     Calculates final drive speed [RPM].
 
@@ -191,15 +189,16 @@
     :return:
         Final drive torque losses [N*m].
     :rtype: numpy.array | float
     """
 
     eff_fd = final_drive_efficiency - (n_wheel_drive - 2) / 100
     to = final_drive_torques_out
-    return (1 - eff_fd) / (eff_fd * final_drive_ratio_vector) * to
+    losses_perc = (1 - eff_fd) / (eff_fd)
+    return np.where(to < 0, -losses_perc, losses_perc) * (to / final_drive_ratio_vector)
 
 
 def calculate_final_drive_torques_in(
     final_drive_torques_out, final_drive_ratio_vector, final_drive_torque_losses
 ):
     """
     Calculates final drive torque [N*m].
@@ -459,23 +458,23 @@
 #     return -engine_wfb_idle / engine_wfa_idle
 
 
 def calculate_fuel_ABC(params, mean_piston_speed, n_powers, n_temperatures):
     p = params
     A = p["a2"] + p["b2"] * mean_piston_speed
     B = p["a"] + (p["b"] + p["c"] * mean_piston_speed) * mean_piston_speed
-    C = numpy.power(n_temperatures, 0) * (p["l"] + p["l2"] * mean_piston_speed**2)
+    C = np.power(n_temperatures, 0) * (p["l"] + p["l2"] * mean_piston_speed**2)
     C -= n_powers
 
     return A, B, C
 
 
 def calculate_VMEP(A, B, C):
-    if (B**2 - 4 * A * C) < 0:
-        print("Negative (B ** 2 - 4 * A * C) ")
+    # if (B ** 2 - 4 * A * C) < 0:
+    #     print('Negative (B ** 2 - 4 * A * C) ')
     if A != 0 and (B**2 - 4 * A * C) >= 0:
         res = (-B + math.sqrt(B**2 - 4 * A * C)) / (2 * A)
     else:
         res = float(-C) / B
     return res
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/gear_functions.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/gear_functions.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/generic_co2mpas.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/generic_co2mpas.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     slope,
     gear,
     gear_count,
     sim_step,
 ):
     n_wheel_drive = car_type
 
+    if fuel_type == "electricity":
+        return 0
+
     # The power on wheels in kW
     veh_wheel_power = func.calculate_wheel_power(
         speed, acceleration, road_loads, vehicle_mass, slope
     )
 
     # The speed on the wheels in [RPM]
     veh_wheel_speed = func.calculate_wheel_speeds(speed, r_dynamic)
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/plot_templates.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/plot_templates.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/reading_n_organizing.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/reading_n_organizing.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/simulation_part.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/simulation_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     :param gear_count:
     :param acc:
     :param my_car:
     :return:
     """
 
     if gear_count > 0:
-
         if my_car.transmission == "manual":
             return 0.0
         else:
             return acc * 2 / 3
     else:
         return acc
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/utils.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,14 @@
         Gear vector corrected from fluctuations.
     :rtype: numpy.array
     """
 
     xy = [list(v) for v in zip(times, gears)]
 
     for samples in sliding_window(xy, dt_window):
-
         up, dn = False, False
 
         x, y = zip(*samples)
 
         for k, d in enumerate(np.diff(y)):
             if d > 0:
                 up = True
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/vehicle_functions.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_functions.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/common/vehicle_specs_class.py` & `co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_specs_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Define veh_specs class"""
 
 
 class veh_specs(object):
-
     # The class "constructor"
     def __init__(self, my_car, **kwargs):
         """
         kwargs can be:
         lco = True          # Light co2mpas is to be used, so the relevant parameters must be imported
         electric = True     # The vehicle is an EV
 
@@ -179,7 +178,18 @@
             "biodiesel": 37900.0,
         }
 
         self.idle_engine_speed_median = {
             "petrol": self.min_engine_on_speed + 300,
             "diesel": self.min_engine_on_speed + 200,
         }
+
+        self.CARBON_CONTENT = {
+            "petrol": 3.17,
+            "diesel": 3.16,
+            "LPG": 1.35,
+            "NG": 3.21,
+            "ethanol": 1.91,
+            "methanol": 1.37,
+            "propane": 2.99,
+            "biodiesel": 2.81,
+        }
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/db/EuroSegmentCar.csv` & `co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar.csv`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/db/EuroSegmentCar_cleaned.csv` & `co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned.csv`

 * *Files 6% similar despite different names*

```diff
@@ -527,1587 +527,1587 @@
 000020e0: 2c33 3133 2e39 3830 3538 3235 2c5b 332e  ,313.9805825,[3.
 000020f0: 3733 2d20 322e 3035 2d20 312e 3336 2d20  73- 2.05- 1.36- 
 00002100: 312e 3033 2d20 302e 3832 2d20 302e 3639  1.03- 0.82- 0.69
 00002110: 5d2c 3132 3333 2e38 3735 2c31 3330 382e  ],1233.875,1308.
 00002120: 3837 352c 3133 3333 2e38 3735 2c31 3235  875,1333.875,125
 00002130: 302c 322e 3730 3533 3332 2c43 0d0a 3437  0,2.705332,C..47
 00002140: 3834 342c 432c 2c79 6573 2c79 6573 2c79  844,C,,yes,yes,y
-00002150: 6573 2c79 6573 2c79 6573 2c79 6573 2c80  es,yes,yes,yes,.
-00002160: 2033 3030 2e30 302c 7965 732c 6e6f 2c2c   300.00,yes,no,,
-00002170: 656c 6563 7472 6963 2065 6e67 696e 652c  electric engine,
-00002180: 656c 6563 7472 6963 6974 792c 3130 372c  electricity,107,
-00002190: 3235 302c 6672 6f6e 742c 3233 2c6c 6974  250,front,23,lit
-000021a0: 6869 756d 2d69 6f6e 2c2c 2c70 6572 6d61  hium-ion,,,perma
-000021b0: 6e65 6e74 206d 6167 6e65 7420 7379 6e63  nent magnet sync
-000021c0: 6872 6f6e 6f75 7320 6d6f 746f 722c 3235  hronous motor,25
-000021d0: 302c 312c 3130 372c 3136 322c 2c31 2e34  0,1,107,162,,1.4
-000021e0: 3636 2c34 2e33 3538 2c32 2e36 3438 2c31  66,4.358,2.648,1
-000021f0: 2e38 3233 2c2c 2c2c 2c2c 2c2c 2c2c 2c2c  .823,,,,,,,,,,,,
-00002200: 2c2c 6861 7463 6862 6163 6b2c 352c 3230  ,,hatchback,5,20
-00002210: 3134 2c33 3939 3930 2c35 2c32 3031 332c  14,39990,5,2013,
-00002220: 7369 6e67 6c65 2d73 7065 6564 2066 6978  single-speed fix
-00002230: 6564 2067 6561 722c 3131 2e34 2c2c 302c  ed gear,11.4,,0,
-00002240: 412c 2c31 3335 2c2c 372e 3832 2c2c 3136  A,,135,,7.82,,16
-00002250: 3434 2c2c 2c2c 3332 332e 342c 2c2c 3136  44,,,,323.4,,,16
-00002260: 3434 2c2c 2c2c 322e 3637 3235 3138 2c43  44,,,,2.672518,C
-00002270: 0d0a 3339 3732 332c 432c 3536 3530 312c  ..39723,C,56501,
-00002280: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
-00002290: 2c6e 6f2c 7965 732c 7965 732c 7965 732c  ,no,yes,yes,yes,
-000022a0: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
-000022b0: 726f 6c2c 3936 2c32 3330 2c66 726f 6e74  rol,96,230,front
-000022c0: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3731  ,,,,,,,,,,,1.471
-000022d0: 2c34 2e35 3835 2c32 2e37 332c 312e 3830  ,4.585,2.73,1.80
-000022e0: 342c 2c31 3139 392c 7265 6775 6c61 722c  4,,1199,regular,
-000022f0: 332c 646f 6863 2c6d 756c 7469 706f 696e  3,dohc,multipoin
-00002300: 7420 696e 6a65 6374 696f 6e2c 3533 2c35  t injection,53,5
-00002310: 3530 302c 3936 2c31 3735 302c 3233 302c  500,96,1750,230,
-00002320: 7965 732c 342c 7374 6174 696f 6e77 6167  yes,4,stationwag
-00002330: 6f6e 2c35 2c61 7661 696c 6162 6c65 2c32  on,5,available,2
-00002340: 3930 3130 2c35 2c32 3031 352c 6d61 6e75  9010,5,2015,manu
-00002350: 616c 2c31 302c 342e 372c 3130 392c 412c  al,10,4.7,109,A,
-00002360: 342c 3230 352c 352e 392c 342e 3138 2c32  4,205,5.9,4.18,2
-00002370: 3435 302c 3131 3635 2c31 3834 302c 3830  450,1165,1840,80
-00002380: 2c39 302e 352c 3239 342e 3837 352c 3330  ,90.5,294.875,30
-00002390: 372e 3931 3236 3231 342c 5b33 2e35 342d  7.9126214,[3.54-
-000023a0: 2031 2e39 322d 2031 2e32 322d 2030 2e38   1.92- 1.22- 0.8
-000023b0: 362d 2030 2e37 2d20 302e 3539 5d2c 3131  6- 0.7- 0.59],11
-000023c0: 3239 2e32 3235 2c31 3230 342e 3232 352c  29.225,1204.225,
-000023d0: 3132 3239 2e32 3235 2c31 3235 302c 322e  1229.225,1250,2.
-000023e0: 3635 3336 3834 2c43 0d0a 3334 3039 322c  653684,C..34092,
-000023f0: 432c 3438 3533 352c 7965 732c 7965 732c  C,48535,yes,yes,
-00002400: 7965 732c 7965 732c 2c79 6573 2c79 6573  yes,yes,,yes,yes
-00002410: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
-00002420: 6e67 696e 652c 6469 6573 656c 2c31 3333  ngine,diesel,133
-00002430: 2c34 3030 2c66 726f 6e74 2c2c 2c2c 2c2c  ,400,front,,,,,,
-00002440: 2c2c 2c2c 2c31 2e34 3537 2c34 2e32 3533  ,,,,,1.457,4.253
-00002450: 2c32 2e36 322c 312e 3830 342c 2c31 3939  ,2.62,1.804,,199
-00002460: 372c 7061 7274 6963 6c65 2066 696c 7465  7,particle filte
-00002470: 722c 342c 646f 6863 2c63 6f6d 6d6f 6e20  r,4,dohc,common 
-00002480: 7261 696c 2c35 332c 3337 3530 2c31 3333  rail,53,3750,133
-00002490: 2c32 3030 302c 3430 302c 7965 732c 342c  ,2000,400,yes,4,
-000024a0: 6861 7463 6862 6163 6b2c 352c 6176 6169  hatchback,5,avai
-000024b0: 6c61 626c 652c 3335 3333 302c 352c 3230  lable,35330,5,20
-000024c0: 3135 2c61 7574 6f6d 6174 6963 2c38 2e34  15,automatic,8.4
-000024d0: 2c34 2c31 3033 2c43 2c33 2e35 2c32 3230  ,4,103,C,3.5,220
-000024e0: 2c34 2e37 2c32 2e39 352c 3139 3530 2c31  ,4.7,2.95,1950,1
-000024f0: 3239 352c 3139 3230 2c2c 3838 2c32 3938  295,1920,,88,298
-00002500: 2e38 2c33 3039 2e33 3230 3338 3833 2c5b  .8,309.3203883,[
-00002510: 342e 3435 2d20 322e 352d 2031 2e35 362d  4.45- 2.5- 1.56-
-00002520: 2031 2e31 342d 2030 2e38 352d 2030 2e36   1.14- 0.85- 0.6
-00002530: 375d 2c31 3235 392e 3232 352c 3133 3334  7],1259.225,1334
-00002540: 2e32 3235 2c31 3335 392e 3232 352c 3133  .225,1359.225,13
-00002550: 3630 2c32 2e36 3238 3432 382c 430d 0a32  60,2.628428,C..2
-00002560: 3539 322c 432c 3335 3634 2c79 6573 2c79  592,C,3564,yes,y
-00002570: 6573 2c79 6573 2c79 6573 2c2c 7965 732c  es,yes,yes,,yes,
-00002580: 3536 302c 7965 732c 7965 732c 2c66 7565  560,yes,yes,,fue
-00002590: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
-000025a0: 3831 2c32 3530 2c66 726f 6e74 2c2c 2c2c  81,250,front,,,,
-000025b0: 2c2c 2c2c 2c2c 2c31 2e34 3231 2c34 2e32  ,,,,,,,1.421,4.2
-000025c0: 3337 2c32 2e36 3031 2c31 2e37 3737 2c2c  37,2.601,1.777,,
-000025d0: 3135 3938 2c70 6172 7469 636c 6520 6669  1598,particle fi
-000025e0: 6c74 6572 2c34 2c64 6f68 632c 636f 6d6d  lter,4,dohc,comm
-000025f0: 6f6e 2072 6169 6c2c 3530 2c33 3230 302c  on rail,50,3200,
-00002600: 3831 2c31 3530 302c 3235 302c 7965 732c  81,1500,250,yes,
-00002610: 342c 6861 7463 6862 6163 6b2c 332c 6176  4,hatchback,3,av
-00002620: 6169 6c61 626c 652c 3333 3734 302c 352c  ailable,33740,5,
-00002630: 3230 3134 2c6d 616e 7561 6c2c 3130 2e35  2014,manual,10.5
-00002640: 2c33 2e38 2c39 392c 432c 332e 342c 3230  ,3.8,99,C,3.4,20
-00002650: 302c 342e 352c 332e 3339 2c32 3030 302c  0,4.5,3.39,2000,
-00002660: 3132 3035 2c31 3739 302c 3735 2c38 302e  1205,1790,75,80.
-00002670: 352c 3239 342e 3837 352c 3330 372e 3931  5,294.875,307.91
-00002680: 3236 3231 342c 5b34 2e31 312d 2032 2e31  26214,[4.11- 2.1
-00002690: 322d 2031 2e33 362d 2030 2e39 372d 2030  2- 1.36- 0.97- 0
-000026a0: 2e37 332d 2030 2e35 395d 2c31 3137 312e  .73- 0.59],1171.
-000026b0: 3235 2c31 3234 362e 3235 2c31 3237 312e  25,1246.25,1271.
-000026c0: 3235 2c31 3235 302c 322e 3532 3531 3137  25,1250,2.525117
-000026d0: 2c43 0d0a 3536 3335 2c43 2c36 3931 312c  ,C..5635,C,6911,
-000026e0: 7965 732c 7965 732c 7965 732c 6e6f 2c2c  yes,yes,yes,no,,
-000026f0: 6e6f 2c6e 6f2c 7965 732c 6e6f 2c2c 6675  no,no,yes,no,,fu
-00002700: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
-00002710: 2c38 312c 3230 352c 6672 6f6e 742c 2c2c  ,81,205,front,,,
-00002720: 2c2c 2c2c 2c2c 2c2c 312e 3438 392c 342e  ,,,,,,,,1.489,4.
-00002730: 3332 392c 322e 3630 382c 312e 3738 392c  329,2.608,1.789,
-00002740: 2c31 3139 392c 7265 6775 6c61 722c 332c  ,1199,regular,3,
-00002750: 646f 6863 2c64 6972 6563 7420 696e 6a65  dohc,direct inje
-00002760: 6374 696f 6e2c 3630 2c35 3530 302c 3831  ction,60,5500,81
-00002770: 2c31 3735 302c 3230 352c 7965 732c 342c  ,1750,205,yes,4,
-00002780: 6861 7463 6862 6163 6b2c 352c 6176 6169  hatchback,5,avai
-00002790: 6c61 626c 652c 3139 3739 302c 352c 3230  lable,19790,5,20
-000027a0: 3135 2c6d 616e 7561 6c2c 3132 2e33 2c34  15,manual,12.3,4
-000027b0: 2e38 2c31 3132 2c41 2c34 2c31 3834 2c36  .8,112,A,4,184,6
-000027c0: 2e31 2c34 2e39 332c 3337 3030 2c31 3137  .1,4.93,3700,117
-000027d0: 352c 3137 3730 2c37 352c 3930 2e35 2c32  5,1770,75,90.5,2
-000027e0: 3839 2e33 3635 2c33 3038 2e30 3039 3730  89.365,308.00970
-000027f0: 3837 2c5b 332e 3436 2d20 312e 3837 2d20  87,[3.46- 1.87- 
-00002800: 312e 3239 2d20 302e 3935 2d20 302e 3735  1.29- 0.95- 0.75
-00002810: 5d2c 3131 3334 2e35 2c31 3230 392e 352c  ],1134.5,1209.5,
-00002820: 3132 3334 2e35 2c31 3235 302c 322e 3636  1234.5,1250,2.66
-00002830: 3338 3231 2c43 0d0a 3536 3330 2c43 2c36  3821,C..5630,C,6
-00002840: 3930 342c 7965 732c 7965 732c 7965 732c  904,yes,yes,yes,
-00002850: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-00002860: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-00002870: 2c64 6965 7365 6c2c 3838 2c33 3030 2c66  ,diesel,88,300,f
-00002880: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
-00002890: 2e34 3839 2c34 2e33 3239 2c32 2e36 3038  .489,4.329,2.608
-000028a0: 2c31 2e37 3839 2c2c 3135 3630 2c70 6172  ,1.789,,1560,par
-000028b0: 7469 636c 6520 6669 6c74 6572 2c34 2c64  ticle filter,4,d
-000028c0: 6f68 632c 636f 6d6d 6f6e 2072 6169 6c2c  ohc,common rail,
-000028d0: 3630 2c33 3530 302c 3838 2c31 3735 302c  60,3500,88,1750,
-000028e0: 3330 302c 7965 732c 322c 6861 7463 6862  300,yes,2,hatchb
-000028f0: 6163 6b2c 352c 6176 6169 6c61 626c 652c  ack,5,available,
-00002900: 3236 3339 302c 352c 3230 3135 2c6d 616e  26390,5,2015,man
-00002910: 7561 6c2c 3130 2e36 2c33 2e36 2c39 332c  ual,10.6,3.6,93,
-00002920: 422c 332e 332c 3139 372c 342e 312c 332e  B,3.3,197,4.1,3.
-00002930: 3734 2c32 3130 302c 3132 3535 2c31 3836  74,2100,1255,186
-00002940: 302c 3535 2c38 382e 332c 3239 312e 3134  0,55,88.3,291.14
-00002950: 352c 3330 362e 3734 3735 3732 382c 5b33  5,306.7475728,[3
-00002960: 2e35 342d 2031 2e39 322d 2031 2e32 382d  .54- 1.92- 1.28-
-00002970: 2030 2e39 312d 2030 2e36 372d 2030 2e35   0.91- 0.67- 0.5
-00002980: 365d 2c31 3231 342e 352c 3132 3839 2e35  6],1214.5,1289.5
-00002990: 2c31 3331 342e 352c 3132 3530 2c32 2e36  ,1314.5,1250,2.6
-000029a0: 3633 3832 312c 430d 0a37 3636 312c 432c  63821,C..7661,C,
-000029b0: 3931 3933 2c79 6573 2c79 6573 2c79 6573  9193,yes,yes,yes
-000029c0: 2c6e 6f2c 2c6e 6f2c 3339 352c 7965 732c  ,no,,no,395,yes,
-000029d0: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
-000029e0: 7065 7472 6f6c 2c31 3235 2c32 3630 2c66  petrol,125,260,f
-000029f0: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
-00002a00: 2e35 312c 342e 3431 392c 322e 3638 352c  .51,4.419,2.685,
-00002a10: 312e 3831 342c 2c31 3539 382c 7265 6775  1.814,,1598,regu
-00002a20: 6c61 722c 342c 646f 6863 2c64 6972 6563  lar,4,dohc,direc
-00002a30: 7420 696e 6a65 6374 696f 6e2c 3536 2c36  t injection,56,6
-00002a40: 3030 302c 3132 352c 3136 3530 2c32 3630  000,125,1650,260
-00002a50: 2c79 6573 2c34 2c68 6174 6368 6261 636b  ,yes,4,hatchback
-00002a60: 2c35 2c61 7661 696c 6162 6c65 2c32 3638  ,5,available,268
-00002a70: 3435 2c35 2c32 3031 352c 6d61 6e75 616c  45,5,2015,manual
-00002a80: 2c38 2e37 2c35 2e39 2c31 3339 2c43 2c34  ,8.7,5.9,139,C,4
-00002a90: 2e39 2c32 3230 2c37 2e38 2c33 2e38 332c  .9,220,7.8,3.83,
-00002aa0: 3237 3530 2c31 3333 302c 3230 3030 2c37  2750,1330,2000,7
-00002ab0: 352c 3831 2e35 2c33 3033 2e36 352c 3331  5,81.5,303.65,31
-00002ac0: 382e 3833 3439 3531 352c 5b33 2e38 322d  8.8349515,[3.82-
-00002ad0: 2032 2e31 362d 2031 2e34 382d 2031 2e30   2.16- 1.48- 1.0
-00002ae0: 372d 2030 2e38 382d 2030 2e37 345d 2c31  7- 0.88- 0.74],1
-00002af0: 3239 322e 322c 3133 3637 2e32 2c31 3339  292.2,1367.2,139
-00002b00: 322e 322c 3133 3630 2c32 2e37 3339 3134  2.2,1360,2.73914
-00002b10: 2c43 0d0a 3736 3833 2c43 2c39 3231 352c  ,C..7683,C,9215,
-00002b20: 7965 732c 7965 732c 7965 732c 6e6f 2c2c  yes,yes,yes,no,,
-00002b30: 6e6f 2c33 3935 2c79 6573 2c79 6573 2c2c  no,395,yes,yes,,
-00002b40: 6675 656c 2065 6e67 696e 652c 6469 6573  fuel engine,dies
-00002b50: 656c 2c31 3231 2c33 3530 2c66 726f 6e74  el,121,350,front
-00002b60: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35 312c  ,,,,,,,,,,,1.51,
-00002b70: 342e 3431 392c 322e 3638 352c 312e 3831  4.419,2.685,1.81
-00002b80: 342c 2c31 3935 362c 7061 7274 6963 6c65  4,,1956,particle
-00002b90: 2066 696c 7465 722c 342c 6f68 632c 636f   filter,4,ohc,co
-00002ba0: 6d6d 6f6e 2072 6169 6c2c 3536 2c34 3030  mmon rail,56,400
-00002bb0: 302c 3132 312c 3137 3530 2c33 3530 2c79  0,121,1750,350,y
-00002bc0: 6573 2c34 2c68 6174 6368 6261 636b 2c35  es,4,hatchback,5
-00002bd0: 2c61 7661 696c 6162 6c65 2c32 3934 3935  ,available,29495
-00002be0: 2c35 2c32 3031 352c 6d61 6e75 616c 2c39  ,5,2015,manual,9
-00002bf0: 2c34 2e35 2c31 3139 2c44 2c34 2c32 3135  ,4.5,119,D,4,215
-00002c00: 2c35 2e34 2c33 2e33 352c 3230 3030 2c31  ,5.4,3.35,2000,1
-00002c10: 3431 382c 3230 3430 2c37 352c 3930 2e34  418,2040,75,90.4
-00002c20: 2c33 3033 2e36 352c 3331 382e 3833 3439  ,303.65,318.8349
-00002c30: 3531 352c 5b34 2e31 372d 2032 2e31 332d  515,[4.17- 2.13-
-00002c40: 2031 2e33 322d 2030 2e39 352d 2030 2e37   1.32- 0.95- 0.7
-00002c50: 352d 2030 2e36 325d 2c31 3338 302e 322c  5- 0.62],1380.2,
-00002c60: 3134 3535 2e32 2c31 3438 302e 322c 3134  1455.2,1480.2,14
-00002c70: 3730 2c32 2e37 3339 3134 2c43 0d0a 3837  70,2.73914,C..87
-00002c80: 3039 2c43 2c31 3038 3330 2c79 6573 2c79  09,C,10830,yes,y
-00002c90: 6573 2c6e 6f2c 6e6f 2c2c 6e6f 2c6e 6f2c  es,no,no,,no,no,
-00002ca0: 7965 732c 7965 732c 2c66 7565 6c20 656e  yes,yes,,fuel en
-00002cb0: 6769 6e65 2c70 6574 726f 6c2c 3939 2c31  gine,petrol,99,1
-00002cc0: 3634 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  64,front,,,,,,,,
-00002cd0: 2c2c 2c31 2e34 3635 2c34 2e33 2c32 2e36  ,,,1.465,4.3,2.6
-00002ce0: 352c 312e 3738 2c2c 3135 3931 2c72 6567  5,1.78,,1591,reg
-00002cf0: 756c 6172 2c34 2c64 6f68 632c 6469 7265  ular,4,dohc,dire
-00002d00: 6374 2069 6e6a 6563 7469 6f6e 2c35 332c  ct injection,53,
-00002d10: 3633 3030 2c39 392c 3438 3530 2c31 3634  6300,99,4850,164
-00002d20: 2c6e 6f2c 342c 6861 7463 6862 6163 6b2c  ,no,4,hatchback,
-00002d30: 352c 6176 6169 6c61 626c 652c 3139 3939  5,available,1999
-00002d40: 352c 352c 3230 3134 2c6d 616e 7561 6c2c  5,5,2014,manual,
-00002d50: 392e 392c 352c 3131 382c 422c 342e 332c  9.9,5,118,B,4.3,
-00002d60: 3139 302c 362e 342c 342e 3036 2c32 3830  190,6.4,4.06,280
-00002d70: 302c 3131 3638 2c31 3732 302c 3830 2c38  0,1168,1720,80,8
-00002d80: 352e 342c 3238 392e 3336 352c 3330 382e  5.4,289.365,308.
-00002d90: 3030 3937 3038 372c 5b33 2e37 372d 2032  0097087,[3.77- 2
-00002da0: 2e30 352d 2031 2e33 372d 2031 2e30 342d  .05- 1.37- 1.04-
-00002db0: 2030 2e38 342d 2030 2e36 395d 2c31 3133   0.84- 0.69],113
-00002dc0: 322e 3232 352c 3132 3037 2e32 3235 2c31  2.225,1207.225,1
-00002dd0: 3233 322e 3232 352c 3132 3530 2c32 2e36  232.225,1250,2.6
-00002de0: 3037 372c 430d 0a39 3736 392c 432c 3132  077,C..9769,C,12
-00002df0: 3037 322c 7965 732c 7965 732c 7965 732c  072,yes,yes,yes,
-00002e00: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-00002e10: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-00002e20: 2c64 6965 7365 6c2c 3934 2c32 3630 2c66  ,diesel,94,260,f
-00002e30: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
-00002e40: 2e34 3635 2c34 2e33 2c32 2e36 352c 312e  .465,4.3,2.65,1.
-00002e50: 3738 2c2c 3135 3832 2c70 6172 7469 636c  78,,1582,particl
-00002e60: 6520 6669 6c74 6572 2c34 2c64 6f68 632c  e filter,4,dohc,
-00002e70: 636f 6d6d 6f6e 2072 6169 6c2c 3533 2c34  common rail,53,4
-00002e80: 3030 302c 3934 2c31 3930 302c 3236 302c  000,94,1900,260,
-00002e90: 7965 732c 342c 6861 7463 6862 6163 6b2c  yes,4,hatchback,
-00002ea0: 332c 3230 3134 2c32 3537 3935 2c35 2c32  3,2014,25795,5,2
-00002eb0: 3031 332c 6d61 6e75 616c 2c31 302e 392c  013,manual,10.9,
-00002ec0: 332e 372c 3937 2c43 2c33 2e35 2c31 3838  3.7,97,C,3.5,188
-00002ed0: 2c34 2e31 2c33 2e34 372c 3231 3030 2c31  ,4.1,3.47,2100,1
-00002ee0: 3236 352c 3138 3130 2c38 302c 3835 2c32  265,1810,80,85,2
-00002ef0: 3931 2e31 3435 2c33 3036 2e37 3437 3537  91.145,306.74757
-00002f00: 3238 2c5b 332e 3737 2d20 322e 3035 2d20  28,[3.77- 2.05- 
-00002f10: 312e 3139 2d20 302e 3834 2d20 302e 372d  1.19- 0.84- 0.7-
-00002f20: 2030 2e36 5d2c 3132 3239 2e32 3235 2c31   0.6],1229.225,1
-00002f30: 3330 342e 3232 352c 3133 3239 2e32 3235  304.225,1329.225
-00002f40: 2c31 3235 302c 322e 3630 3737 2c43 0d0a  ,1250,2.6077,C..
-00002f50: 3138 3732 2c43 2c32 3833 342c 7965 732c  1872,C,2834,yes,
-00002f60: 7965 732c 7965 732c 7965 732c 2c6e 6f2c  yes,yes,yes,,no,
-00002f70: 7965 732c 7965 732c 7965 732c 2c66 7565  yes,yes,yes,,fue
-00002f80: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
-00002f90: 3838 2c32 3830 2c66 726f 6e74 2c2c 2c2c  88,280,front,,,,
-00002fa0: 2c2c 2c2c 2c2c 2c31 2e34 372c 342e 3337  ,,,,,,,1.47,4.37
-00002fb0: 2c32 2e36 3436 2c31 2e38 3032 2c2c 3139  ,2.646,1.802,,19
-00002fc0: 3639 2c70 6172 7469 636c 6520 6669 6c74  69,particle filt
-00002fd0: 6572 2c34 2c64 6f68 632c 636f 6d6d 6f6e  er,4,dohc,common
-00002fe0: 2072 6169 6c2c 3532 2c33 3735 302c 3838   rail,52,3750,88
-00002ff0: 2c31 3530 302c 3238 302c 7965 732c 342c  ,1500,280,yes,4,
-00003000: 6861 7463 6862 6163 6b2c 352c 6176 6169  hatchback,5,avai
-00003010: 6c61 626c 652c 3337 3939 352c 352c 3230  lable,37995,5,20
-00003020: 3135 2c6d 616e 7561 6c2c 3130 2e36 2c33  15,manual,10.6,3
-00003030: 2e37 2c39 362c 422c 332e 342c 3139 302c  .7,96,B,3.4,190,
-00003040: 342e 322c 332e 3631 2c32 3135 302c 3133  4.2,3.61,2150,13
-00003050: 3438 2c31 3938 302c 3130 302c 3933 2e32  48,1980,100,93.2
-00003060: 2c33 3033 2e36 352c 3331 382e 3833 3439  ,303.65,318.8349
-00003070: 3531 352c 5b33 2e37 332d 2032 2e30 352d  515,[3.73- 2.05-
-00003080: 2031 2e32 362d 2030 2e39 322d 2030 2e37   1.26- 0.92- 0.7
-00003090: 342d 2030 2e36 325d 2c31 3331 322e 392c  4- 0.62],1312.9,
-000030a0: 3133 3837 2e39 2c31 3431 322e 392c 3133  1387.9,1412.9,13
-000030b0: 3630 2c32 2e36 3438 3934 2c43 0d0a 3130  60,2.64894,C..10
-000030c0: 3332 382c 432c 3133 3536 322c 7965 732c  328,C,13562,yes,
-000030d0: 7965 732c 7965 732c 7965 732c 2c6e 6f2c  yes,yes,yes,,no,
-000030e0: 7965 732c 7965 732c 6e6f 2c2c 6675 656c  yes,yes,no,,fuel
-000030f0: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
-00003100: 3037 2c31 3835 2c66 726f 6e74 2c2c 2c2c  07,185,front,,,,
-00003110: 2c2c 2c2c 2c2c 2c31 2e34 3537 2c34 2e35  ,,,,,,,1.457,4.5
-00003120: 3232 2c32 2e36 342c 312e 3737 2c2c 3139  22,2.64,1.77,,19
-00003130: 3939 2c72 6567 756c 6172 2c34 2c64 6f68  99,regular,4,doh
-00003140: 632c 6d75 6c74 6970 6f69 6e74 2069 6e6a  c,multipoint inj
-00003150: 6563 7469 6f6e 2c35 352c 3630 3030 2c31  ection,55,6000,1
-00003160: 3037 2c34 3030 302c 3138 352c 6e6f 2c34  07,4000,185,no,4
-00003170: 2c73 7461 7469 6f6e 7761 676f 6e2c 352c  ,stationwagon,5,
-00003180: 3230 3132 2c33 3137 3530 2c35 2c32 3031  2012,31750,5,201
-00003190: 312c 6d61 6e75 616c 2c39 2e36 2c37 2e36  1,manual,9.6,7.6
-000031a0: 2c31 3736 2c46 2c35 2e37 2c32 3130 2c31  ,176,F,5.7,210,1
-000031b0: 302e 382c 342e 3037 2c33 3530 302c 3132  0.8,4.07,3500,12
-000031c0: 3833 2c31 3839 302c 3130 302c 3833 2e31  83,1890,100,83.1
-000031d0: 2c32 3931 2e31 3435 2c33 3036 2e37 3437  ,291.145,306.747
-000031e0: 3537 3238 2c5b 332e 3432 2d20 322e 3134  5728,[3.42- 2.14
-000031f0: 2d20 312e 3438 2d20 312e 3131 2d20 302e  - 1.48- 1.11- 0.
-00003200: 3835 5d2c 3132 3435 2e38 3735 2c31 3332  85],1245.875,132
-00003210: 302e 3837 352c 3133 3435 2e38 3735 2c31  0.875,1345.875,1
-00003220: 3336 302c 322e 3537 3838 392c 430d 0a33  360,2.57889,C..3
-00003230: 3534 3736 2c44 2c35 3033 3536 2c79 6573  5476,D,50356,yes
-00003240: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-00003250: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-00003260: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
-00003270: 2c39 322c 3230 302c 6672 6f6e 742c 2c2c  ,92,200,front,,,
-00003280: 2c2c 2c2c 2c2c 2c2c 312e 3436 312c 342e  ,,,,,,,,1.461,4.
-00003290: 3736 372c 322e 3739 312c 312e 3833 322c  767,2.791,1.832,
-000032a0: 2c31 3339 352c 7265 6775 6c61 722c 342c  ,1395,regular,4,
-000032b0: 646f 6863 2c64 6972 6563 7420 696e 6a65  dohc,direct inje
-000032c0: 6374 696f 6e2c 3636 2c35 3030 302c 3932  ction,66,5000,92
-000032d0: 2c31 3430 302c 3230 302c 7965 732c 342c  ,1400,200,yes,4,
-000032e0: 7365 6461 6e2c 342c 6176 6169 6c61 626c  sedan,4,availabl
-000032f0: 652c 3332 3335 302c 352c 3230 3135 2c6d  e,32350,5,2015,m
-00003300: 616e 7561 6c2c 392e 372c 352e 332c 3132  anual,9.7,5.3,12
-00003310: 332c 412c 342e 342c 3230 382c 362e 382c  3,A,4.4,208,6.8,
-00003320: 342e 3335 2c32 3730 302c 3132 3637 2c31  4.35,2700,1267,1
-00003330: 3931 302c 3130 302c 3830 2c33 3033 2e38  910,100,80,303.8
-00003340: 322c 3332 322e 3532 3432 3731 382c 5b33  2,322.5242718,[3
-00003350: 2e36 322d 2031 2e39 352d 2031 2e32 382d  .62- 1.95- 1.28-
-00003360: 2030 2e39 372d 2030 2e37 382d 2030 2e36   0.97- 0.78- 0.6
-00003370: 355d 2c31 3232 322e 3435 2c31 3239 372e  5],1222.45,1297.
-00003380: 3435 2c31 3332 322e 3435 2c31 3235 302c  45,1322.45,1250,
-00003390: 322e 3637 3635 3532 2c44 0d0a 3431 3938  2.676552,D..4198
-000033a0: 392c 442c 3539 3639 372c 7965 732c 7965  9,D,59697,yes,ye
-000033b0: 732c 7965 732c 7965 732c 2c6e 6f2c 7965  s,yes,yes,,no,ye
-000033c0: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
-000033d0: 656e 6769 6e65 2c64 6965 7365 6c2c 3838  engine,diesel,88
-000033e0: 2c32 3530 2c66 726f 6e74 2c2c 2c2c 2c2c  ,250,front,,,,,,
-000033f0: 2c2c 2c2c 2c31 2e34 3631 2c34 2e37 3637  ,,,,,1.461,4.767
-00003400: 2c32 2e37 3931 2c31 2e38 3332 2c2c 3135  ,2.791,1.832,,15
-00003410: 3938 2c70 6172 7469 636c 6520 6669 6c74  98,particle filt
-00003420: 6572 2c34 2c64 6f68 632c 636f 6d6d 6f6e  er,4,dohc,common
-00003430: 2072 6169 6c2c 3636 2c33 3630 302c 3838   rail,66,3600,88
-00003440: 2c31 3530 302c 3235 302c 7965 732c 342c  ,1500,250,yes,4,
-00003450: 7365 6461 6e2c 342c 6176 6169 6c61 626c  sedan,4,availabl
-00003460: 652c 3334 3835 302c 352c 3230 3135 2c6d  e,34850,5,2015,m
-00003470: 616e 7561 6c2c 3130 2e38 2c34 2c31 3038  anual,10.8,4,108
-00003480: 2c42 2c33 2e36 2c32 3036 2c34 2e37 2c33  ,B,3.6,206,4.7,3
-00003490: 2e36 352c 3230 3530 2c31 3334 342c 3139  .65,2050,1344,19
-000034a0: 3930 2c31 3030 2c38 302e 352c 3330 332e  90,100,80.5,303.
-000034b0: 3832 2c33 3232 2e35 3234 3237 3138 2c5b  82,322.5242718,[
-000034c0: 342e 3131 2d20 322e 3132 2d20 312e 3336  4.11- 2.12- 1.36
-000034d0: 2d20 302e 3937 2d20 302e 3733 2d20 302e  - 0.97- 0.73- 0.
-000034e0: 3539 5d2c 3132 3939 2e34 352c 3133 3734  59],1299.45,1374
-000034f0: 2e34 352c 3133 3939 2e34 352c 3133 3630  .45,1399.45,1360
-00003500: 2c32 2e36 3736 3535 322c 440d 0a32 3637  ,2.676552,D..267
-00003510: 3939 2c44 2c33 3738 3534 2c79 6573 2c79  99,D,37854,yes,y
-00003520: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
-00003530: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
-00003540: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
-00003550: 3235 2c33 3230 2c66 726f 6e74 2b72 6561  25,320,front+rea
-00003560: 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3432  r,,,,,,,,,,,1.42
-00003570: 372c 342e 3730 312c 322e 3830 382c 312e  7,4.701,2.808,1.
-00003580: 3832 362c 2c31 3739 382c 7265 6775 6c61  826,,1798,regula
-00003590: 722c 342c 646f 6863 2c64 6972 6563 7420  r,4,dohc,direct 
-000035a0: 696e 6a65 6374 696f 6e2c 3631 2c33 3830  injection,61,380
-000035b0: 302c 3132 352c 3134 3030 2c33 3230 2c79  0,125,1400,320,y
-000035c0: 6573 2c34 2c73 6564 616e 2c34 2c61 7661  es,4,sedan,4,ava
-000035d0: 696c 6162 6c65 2c34 3130 3235 2c35 2c32  ilable,41025,5,2
-000035e0: 3031 352c 6d61 6e75 616c 2c37 2e39 2c36  015,manual,7.9,6
-000035f0: 2e32 2c31 3334 2c42 2c35 2e32 2c32 3239  .2,134,B,5.2,229
-00003600: 2c38 2e31 2c33 2e36 392c 3232 3530 2c31  ,8.1,3.69,2250,1
-00003610: 3438 302c 3139 3830 2c39 302c 3834 2e31  480,1980,90,84.1
-00003620: 2c32 3939 2e37 3235 2c33 3137 2e34 3237  ,299.725,317.427
-00003630: 3138 3435 2c5b 332e 3738 2d20 322e 3035  1845,[3.78- 2.05
-00003640: 2d20 312e 3332 2d20 302e 3937 2d20 302e  - 1.32- 0.97- 0.
-00003650: 3736 2d20 302e 3633 5d2c 3134 3338 2e38  76- 0.63],1438.8
-00003660: 3235 2c31 3531 332e 3832 352c 3135 3338  25,1513.825,1538
-00003670: 2e38 3235 2c31 3437 302c 322e 3630 3537  .825,1470,2.6057
-00003680: 3032 2c44 0d0a 3236 3835 312c 442c 3337  02,D..26851,D,37
-00003690: 3932 362c 7965 732c 7965 732c 7965 732c  926,yes,yes,yes,
-000036a0: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-000036b0: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-000036c0: 2c64 6965 7365 6c2c 3134 302c 3430 302c  ,diesel,140,400,
-000036d0: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
-000036e0: 2c2c 2c2c 2c31 2e34 3237 2c34 2e37 3031  ,,,,,1.427,4.701
-000036f0: 2c32 2e38 3038 2c31 2e38 3236 2c2c 3139  ,2.808,1.826,,19
-00003700: 3638 2c70 6172 7469 636c 6520 6669 6c74  68,particle filt
-00003710: 6572 2c34 2c64 6f68 632c 636f 6d6d 6f6e  er,4,dohc,common
-00003720: 2072 6169 6c2c 3633 2c34 3230 302c 3134   rail,63,4200,14
-00003730: 302c 3137 3530 2c34 3030 2c79 6573 2c34  0,1750,400,yes,4
-00003740: 2c73 6564 616e 2c34 2c61 7661 696c 6162  ,sedan,4,availab
-00003750: 6c65 2c35 3334 3530 2c35 2c32 3031 342c  le,53450,5,2014,
-00003760: 6175 746f 6d61 7469 632c 372e 332c 352c  automatic,7.3,5,
-00003770: 3133 322c 442c 342e 352c 3233 352c 352e  132,D,4.5,235,5.
-00003780: 392c 342e 3039 2c31 3835 302c 3136 3330  9,4.09,1850,1630
-00003790: 2c32 3230 352c 3930 2c39 352e 352c 3330  ,2205,90,95.5,30
-000037a0: 352e 3034 2c33 3137 2e30 3837 3337 3836  5.04,317.0873786
-000037b0: 2c5b 332e 3639 2d20 322e 3135 2d20 312e  ,[3.69- 2.15- 1.
-000037c0: 3334 2d20 302e 3937 2d20 302e 3734 2d20  34- 0.97- 0.74- 
-000037d0: 302e 3537 2d20 302e 3436 5d2c 3135 3837  0.57- 0.46],1587
-000037e0: 2e34 3735 2c31 3636 322e 3437 352c 3136  .475,1662.475,16
-000037f0: 3837 2e34 3735 2c31 3730 302c 322e 3630  87.475,1700,2.60
-00003800: 3537 3032 2c44 0d0a 3237 3138 392c 442c  5702,D..27189,D,
-00003810: 3338 3434 372c 7965 732c 7965 732c 7965  38447,yes,yes,ye
-00003820: 732c 7965 732c 2c6e 6f2c 7965 732c 7965  s,yes,,no,yes,ye
-00003830: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00003840: 6e65 2c70 6574 726f 6c2c 3136 352c 3335  ne,petrol,165,35
-00003850: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00003860: 2c2c 2c2c 2c2c 2c31 2e33 3931 2c34 2e37  ,,,,,,,1.391,4.7
-00003870: 3132 2c32 2e38 312c 312e 3835 342c 2c31  12,2.81,1.854,,1
-00003880: 3938 342c 7265 6775 6c61 722c 342c 646f  984,regular,4,do
-00003890: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-000038a0: 696f 6e2c 3634 2c34 3530 302c 3136 352c  ion,64,4500,165,
-000038b0: 3135 3030 2c33 3530 2c79 6573 2c34 2c68  1500,350,yes,4,h
-000038c0: 6174 6368 6261 636b 2c35 2c61 7661 696c  atchback,5,avail
-000038d0: 6162 6c65 2c35 3630 3230 2c34 2c32 3031  able,56020,4,201
-000038e0: 342c 6175 746f 6d61 7469 632c 362e 352c  4,automatic,6.5,
-000038f0: 362e 372c 3135 352c 432c 352e 362c 3234  6.7,155,C,5.6,24
-00003900: 352c 382e 352c 342e 3039 2c32 3035 302c  5,8.5,4.09,2050,
-00003910: 3135 3930 2c32 3136 352c 3930 2c39 322e  1590,2165,90,92.
-00003920: 382c 3330 332e 3635 2c33 3138 2e38 3334  8,303.65,318.834
-00003930: 3935 3135 2c5b 332e 3639 2d20 322e 3135  9515,[3.69- 2.15
-00003940: 2d20 312e 3431 2d20 312e 3033 2d20 302e  - 1.41- 1.03- 0.
-00003950: 3739 2d20 302e 3633 2d20 302e 3532 5d2c  79- 0.63- 0.52],
-00003960: 3135 3436 2e38 2c31 3632 312e 382c 3136  1546.8,1621.8,16
-00003970: 3436 2e38 2c31 3539 302c 322e 3537 3839  46.8,1590,2.5789
-00003980: 3134 2c44 0d0a 3233 3830 312c 442c 3332  14,D..23801,D,32
-00003990: 3836 362c 7965 732c 7965 732c 7965 732c  866,yes,yes,yes,
-000039a0: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-000039b0: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
-000039c0: 7065 7472 6f6c 2c31 3235 2c32 3130 2c72  petrol,125,210,r
-000039d0: 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e  ear,,,,,,,,,,,1.
-000039e0: 3338 342c 342e 3631 322c 322e 3736 2c31  384,4.612,2.76,1
-000039f0: 2e37 3832 2c2c 3139 3935 2c72 6567 756c  .782,,1995,regul
-00003a00: 6172 2c34 2c64 6f68 632c 6469 7265 6374  ar,4,dohc,direct
-00003a10: 2069 6e6a 6563 7469 6f6e 2c36 332c 3637   injection,63,67
-00003a20: 3030 2c31 3235 2c34 3235 302c 3231 302c  00,125,4250,210,
-00003a30: 6e6f 2c34 2c63 6162 7269 6f6c 6574 2c32  no,4,cabriolet,2
-00003a40: 2c32 3031 332c 3537 3637 322c 342c 3230  ,2013,57672,4,20
-00003a50: 3133 2c61 7574 6f6d 6174 6963 2c39 2e38  13,automatic,9.8
-00003a60: 2c37 2e33 2c31 3639 2c45 2c35 2e38 2c32  ,7.3,169,E,5.8,2
-00003a70: 3236 2c39 2e38 2c34 2e31 2c32 3830 302c  26,9.8,4.1,2800,
-00003a80: 3136 3030 2c32 3035 352c 2c39 302c 3239  1600,2055,,90,29
-00003a90: 382e 382c 3330 392e 3332 3033 3838 332c  8.8,309.3203883,
-00003aa0: 5b34 2e31 372d 2032 2e33 342d 2031 2e35  [4.17- 2.34- 1.5
-00003ab0: 322d 2031 2e31 342d 2030 2e38 362d 2030  2- 1.14- 0.86- 0
-00003ac0: 2e36 395d 2c31 3535 372e 3437 352c 3136  .69],1557.475,16
-00003ad0: 3332 2e34 3735 2c31 3635 372e 3437 352c  32.475,1657.475,
-00003ae0: 3135 3930 2c32 2e34 3636 3238 382c 440d  1590,2.466288,D.
-00003af0: 0a33 3037 392c 442c 3430 3635 2c79 6573  .3079,D,4065,yes
-00003b00: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-00003b10: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-00003b20: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
-00003b30: 2c38 352c 3237 302c 7265 6172 2c2c 2c2c  ,85,270,rear,,,,
-00003b40: 2c2c 2c2c 2c2c 2c31 2e34 3239 2c34 2e36  ,,,,,,,1.429,4.6
-00003b50: 3234 2c32 2e38 312c 312e 3831 312c 2c31  24,2.81,1.811,,1
-00003b60: 3939 352c 7061 7274 6963 6c65 2066 696c  995,particle fil
-00003b70: 7465 722c 342c 646f 6863 2c63 6f6d 6d6f  ter,4,dohc,commo
-00003b80: 6e20 7261 696c 2c35 372c 3430 3030 2c38  n rail,57,4000,8
-00003b90: 352c 3132 3530 2c32 3730 2c79 6573 2c34  5,1250,270,yes,4
-00003ba0: 2c73 7461 7469 6f6e 7761 676f 6e2c 352c  ,stationwagon,5,
-00003bb0: 6176 6169 6c61 626c 652c 3434 3239 352c  available,44295,
-00003bc0: 352c 3230 3135 2c6d 616e 7561 6c2c 3131  5,2015,manual,11
-00003bd0: 2e32 2c34 2e31 2c31 3039 2c43 2c33 2e37  .2,4.1,109,C,3.7
-00003be0: 2c32 3030 2c34 2e39 2c33 2e32 332c 3230  ,200,4.9,3.23,20
-00003bf0: 3530 2c31 3437 302c 3230 3930 2c37 352c  50,1470,2090,75,
-00003c00: 3930 2c32 3939 2e31 342c 3331 362e 3639  90,299.14,316.69
-00003c10: 3930 3239 312c 5b34 2e30 2d20 322e 3131  90291,[4.0- 2.11
-00003c20: 2d20 312e 3338 2d20 312e 302d 2030 2e37  - 1.38- 1.0- 0.7
-00003c30: 382d 2030 2e36 355d 2c31 3433 312e 3532  8- 0.65],1431.52
-00003c40: 352c 3135 3036 2e35 3235 2c31 3533 312e  5,1506.525,1531.
-00003c50: 3532 352c 3134 3730 2c32 2e35 3837 3931  525,1470,2.58791
-00003c60: 392c 440d 0a33 3635 3235 2c44 2c35 3138  9,D..36525,D,518
-00003c70: 3734 2c79 6573 2c79 6573 2c79 6573 2c6e  74,yes,yes,yes,n
-00003c80: 6f2c 2c6e 6f2c 3435 302c 7965 732c 7965  o,,no,450,yes,ye
-00003c90: 732c 2c66 7565 6c20 656e 6769 6e65 2c70  s,,fuel engine,p
-00003ca0: 6574 726f 6c2c 3838 2c31 3536 2c66 726f  etrol,88,156,fro
-00003cb0: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  nt,,,,,,,,,,,1.4
-00003cc0: 3536 2c34 2e37 3932 2c32 2e38 3137 2c31  56,4.792,2.817,1
-00003cd0: 2e38 3533 2c2c 3135 3938 2c72 6567 756c  .853,,1598,regul
-00003ce0: 6172 2c34 2c64 6f68 632c 6d75 6c74 6970  ar,4,dohc,multip
-00003cf0: 6f69 6e74 2069 6e6a 6563 7469 6f6e 2c37  oint injection,7
-00003d00: 322c 3630 3030 2c38 382c 3432 3530 2c31  2,6000,88,4250,1
-00003d10: 3536 2c6e 6f2c 342c 7365 6461 6e2c 342c  56,no,4,sedan,4,
-00003d20: 6176 6169 6c61 626c 652c 3239 3038 302c  available,29080,
-00003d30: 352c 3230 3134 2c61 7574 6f6d 6174 6963  5,2014,automatic
-00003d40: 2c31 312e 352c 362e 322c 3134 342c 422c  ,11.5,6.2,144,B,
-00003d50: 342e 362c 3230 332c 392c 342e 3837 2c33  4.6,203,9,4.87,3
-00003d60: 3035 302c 3133 3635 2c31 3934 352c 3730  050,1365,1945,70
-00003d70: 2c38 352e 382c 3330 332e 3832 2c33 3232  ,85.8,303.82,322
-00003d80: 2e35 3234 3237 3138 2c5b 332e 3534 2d20  .5242718,[3.54- 
-00003d90: 312e 3932 2d20 312e 3332 2d20 302e 3938  1.92- 1.32- 0.98
-00003da0: 2d20 302e 3736 2d20 302e 3635 5d2c 3133  - 0.76- 0.65],13
-00003db0: 3136 2e34 2c31 3339 312e 342c 3134 3136  16.4,1391.4,1416
-00003dc0: 2e34 2c31 3336 302c 322e 3639 3739 3638  .4,1360,2.697968
-00003dd0: 2c44 0d0a 3437 3736 362c 442c 3638 3130  ,D..47766,D,6810
-00003de0: 342c 7965 732c 7965 732c 7965 732c 7965  4,yes,yes,yes,ye
-00003df0: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
-00003e00: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
-00003e10: 6965 7365 6c2c 3838 2c33 3030 2c66 726f  iesel,88,300,fro
-00003e20: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  nt,,,,,,,,,,,1.4
-00003e30: 3736 2c34 2e38 3133 2c32 2e38 3137 2c31  76,4.813,2.817,1
-00003e40: 2e38 3533 2c2c 3135 3630 2c70 6172 7469  .853,,1560,parti
-00003e50: 636c 6520 6669 6c74 6572 2c34 2c64 6f68  cle filter,4,doh
-00003e60: 632c 636f 6d6d 6f6e 2072 6169 6c2c 3732  c,common rail,72
-00003e70: 2c33 3530 302c 3838 2c31 3735 302c 3330  ,3500,88,1750,30
-00003e80: 302c 7965 732c 322c 7374 6174 696f 6e77  0,yes,2,stationw
-00003e90: 6167 6f6e 2c35 2c61 7661 696c 6162 6c65  agon,5,available
-00003ea0: 2c33 3533 3630 2c35 2c32 3031 352c 6d61  ,35360,5,2015,ma
-00003eb0: 6e75 616c 2c31 312e 362c 342e 322c 3130  nual,11.6,4.2,10
-00003ec0: 302c 412c 332e 372c 3139 372c 352c 342e  0,A,3.7,197,5,4.
-00003ed0: 3035 2c32 3330 302c 3134 3035 2c32 3130  05,2300,1405,210
-00003ee0: 302c 3830 2c38 382e 332c 3330 332e 3832  0,80,88.3,303.82
-00003ef0: 2c33 3232 2e35 3234 3237 3138 2c5b 332e  ,322.5242718,[3.
-00003f00: 3534 2d20 312e 3932 2d20 312e 3332 2d20  54- 1.92- 1.32- 
-00003f10: 302e 3938 2d20 302e 3736 2d20 302e 365d  0.98- 0.76- 0.6]
-00003f20: 2c31 3335 362e 342c 3134 3331 2e34 2c31  ,1356.4,1431.4,1
-00003f30: 3435 362e 342c 3134 3730 2c32 2e37 3335  456.4,1470,2.735
-00003f40: 3032 382c 440d 0a36 3338 362c 442c 3737  028,D..6386,D,77
-00003f50: 3836 2c79 6573 2c79 6573 2c79 6573 2c79  86,yes,yes,yes,y
-00003f60: 6573 2c2c 7965 732c 7965 732c 7965 732c  es,,yes,yes,yes,
-00003f70: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
-00003f80: 7065 7472 6f6c 2c31 3138 2c32 3430 2c66  petrol,118,240,f
-00003f90: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
-00003fa0: 2e34 3832 2c34 2e38 3731 2c32 2e38 352c  .482,4.871,2.85,
-00003fb0: 312e 3835 322c 2c31 3439 382c 7265 6775  1.852,,1498,regu
-00003fc0: 6c61 722c 342c 646f 6863 2c64 6972 6563  lar,4,dohc,direc
-00003fd0: 7420 696e 6a65 6374 696f 6e2c 3633 2c35  t injection,63,5
-00003fe0: 3730 302c 3131 382c 3136 3030 2c32 3430  700,118,1600,240
-00003ff0: 2c79 6573 2c34 2c68 6174 6368 6261 636b  ,yes,4,hatchback
-00004000: 2c35 2c61 7661 696c 6162 6c65 2c33 3436  ,5,available,346
-00004010: 3935 2c35 2c32 3031 342c 6175 746f 6d61  95,5,2014,automa
-00004020: 7469 632c 392e 312c 362e 332c 3134 362c  tic,9.1,6.3,146,
-00004030: 422c 342e 392c 3231 342c 382e 372c 332e  B,4.9,214,8.7,3.
-00004040: 3037 2c32 3230 302c 3134 3035 2c32 3139  07,2200,1405,219
-00004050: 302c 3735 2c37 362e 342c 3330 332e 3832  0,75,76.4,303.82
-00004060: 2c33 3232 2e35 3234 3237 3138 2c5b 342e  ,322.5242718,[4.
-00004070: 3538 2d20 322e 3936 2d20 312e 3931 2d20  58- 2.96- 1.91- 
-00004080: 312e 3435 2d20 312e 302d 2030 2e37 355d  1.45- 1.0- 0.75]
-00004090: 2c31 3336 322e 3437 352c 3134 3337 2e34  ,1362.475,1437.4
-000040a0: 3735 2c31 3436 322e 3437 352c 3134 3730  75,1462.475,1470
-000040b0: 2c32 2e37 3434 3636 342c 440d 0a33 3339  ,2.744664,D..339
-000040c0: 3538 2c44 2c34 3833 3930 2c79 6573 2c79  58,D,48390,yes,y
-000040d0: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
-000040e0: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
-000040f0: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
-00004100: 3235 2c32 3630 2c66 726f 6e74 2c2c 2c2c  25,260,front,,,,
-00004110: 2c2c 2c2c 2c2c 2c31 2e35 3235 2c34 2e39  ,,,,,,,1.525,4.9
-00004120: 322c 322e 3733 372c 312e 3835 382c 2c31  2,2.737,1.858,,1
-00004130: 3539 382c 7265 6775 6c61 722c 342c 646f  598,regular,4,do
-00004140: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-00004150: 696f 6e2c 3730 2c34 3235 302c 3132 352c  ion,70,4250,125,
-00004160: 3136 3530 2c32 3630 2c79 6573 2c34 2c73  1650,260,yes,4,s
-00004170: 7461 7469 6f6e 7761 676f 6e2c 352c 6176  tationwagon,5,av
-00004180: 6169 6c61 626c 652c 3338 3939 352c 352c  ailable,38995,5,
-00004190: 3230 3134 2c6d 616e 7561 6c2c 392e 382c  2014,manual,9.8,
-000041a0: 362e 322c 3134 362c 422c 352e 332c 3231  6.2,146,B,5.3,21
-000041b0: 352c 372e 382c 332e 3934 2c32 3730 302c  5,7.8,3.94,2700,
-000041c0: 3135 3634 2c32 3231 352c 3130 302c 3831  1564,2215,100,81
-000041d0: 2e35 2c33 3230 2e32 352c 3333 362e 3031  .5,320.25,336.01
-000041e0: 3934 3137 352c 5b34 2e32 372d 2032 2e33  94175,[4.27- 2.3
-000041f0: 352d 2031 2e34 382d 2031 2e30 372d 2030  5- 1.48- 1.07- 0
-00004200: 2e38 382d 2030 2e37 345d 2c31 3531 362e  .88- 0.74],1516.
-00004210: 3735 2c31 3539 312e 3735 2c31 3631 362e  75,1591.75,1616.
-00004220: 3735 2c31 3539 302c 322e 3833 3334 352c  75,1590,2.83345,
-00004230: 440d 0a33 3339 3836 2c44 2c34 3834 3138  D..33986,D,48418
-00004240: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00004250: 2c2c 6e6f 2c79 6573 2c79 6573 2c79 6573  ,,no,yes,yes,yes
-00004260: 2c2c 6675 656c 2065 6e67 696e 652c 6469  ,,fuel engine,di
-00004270: 6573 656c 2c31 3235 2c34 3030 2c66 726f  esel,125,400,fro
-00004280: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35  nt,,,,,,,,,,,1.5
-00004290: 3134 2c34 2e39 3133 2c32 2e37 3337 2c31  14,4.913,2.737,1
-000042a0: 2e38 3538 2c2c 3139 3536 2c70 6172 7469  .858,,1956,parti
-000042b0: 636c 6520 6669 6c74 6572 2c34 2c64 6f68  cle filter,4,doh
-000042c0: 632c 636f 6d6d 6f6e 2072 6169 6c2c 3730  c,common rail,70
-000042d0: 2c33 3530 302c 3132 352c 3137 3530 2c34  ,3500,125,1750,4
-000042e0: 3030 2c79 6573 2c34 2c73 7461 7469 6f6e  00,yes,4,station
-000042f0: 7761 676f 6e2c 352c 6176 6169 6c61 626c  wagon,5,availabl
-00004300: 652c 3433 3039 352c 352c 3230 3135 2c6d  e,43095,5,2015,m
-00004310: 616e 7561 6c2c 392e 392c 342e 352c 3131  anual,9.9,4.5,11
-00004320: 392c 422c 332e 382c 3232 302c 352e 372c  9,B,3.8,220,5.7,
-00004330: 332e 3535 2c32 3035 302c 3136 3333 2c32  3.55,2050,1633,2
-00004340: 3330 302c 3130 302c 3930 2e34 2c33 3134  300,100,90.4,314
-00004350: 2e35 3935 2c33 3238 2e39 3830 3538 3235  .595,328.9805825
-00004360: 2c5b 332e 3932 2d20 322e 3034 2d20 312e  ,[3.92- 2.04- 1.
-00004370: 3332 2d20 302e 3935 2d20 302e 3735 2d20  32- 0.95- 0.75- 
-00004380: 302e 3632 5d2c 3135 3835 2e37 352c 3136  0.62],1585.75,16
-00004390: 3630 2e37 352c 3136 3835 2e37 352c 3137  60.75,1685.75,17
-000043a0: 3030 2c32 2e38 3133 3031 322c 440d 0a35  00,2.813012,D..5
-000043b0: 3732 352c 442c 3730 3335 2c79 6573 2c79  725,D,7035,yes,y
-000043c0: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
-000043d0: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
-000043e0: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
-000043f0: 3231 2c32 3130 2c66 726f 6e74 2c2c 2c2c  21,210,front,,,,
-00004400: 2c2c 2c2c 2c2c 2c31 2e34 382c 342e 382c  ,,,,,,,1.48,4.8,
-00004410: 322e 3735 2c31 2e38 342c 2c31 3939 382c  2.75,1.84,,1998,
-00004420: 7265 6775 6c61 722c 342c 646f 6863 2c64  regular,4,dohc,d
-00004430: 6972 6563 7420 696e 6a65 6374 696f 6e2c  irect injection,
-00004440: 3632 2c36 3030 302c 3132 312c 3430 3030  62,6000,121,4000
-00004450: 2c32 3130 2c6e 6f2c 342c 7374 6174 696f  ,210,no,4,statio
-00004460: 6e77 6167 6f6e 2c35 2c61 7661 696c 6162  nwagon,5,availab
-00004470: 6c65 2c33 3539 3930 2c35 2c32 3031 352c  le,35990,5,2015,
-00004480: 6175 746f 6d61 7469 632c 3130 2e32 2c36  automatic,10.2,6
-00004490: 2c31 3339 2c42 2c35 2c32 3036 2c37 2e37  ,139,B,5,206,7.7
-000044a0: 2c34 2e33 332c 3234 3530 2c31 3331 352c  ,4.33,2450,1315,
-000044b0: 3230 3230 2c2c 3931 2e32 2c33 3132 2e34  2020,,91.2,312.4
-000044c0: 3235 2c33 3239 2e37 3537 3238 3136 2c5b  25,329.7572816,[
-000044d0: 332e 3535 2d20 322e 3032 2d20 312e 3435  3.55- 2.02- 1.45
-000044e0: 2d20 312e 302d 2030 2e37 312d 2030 2e36  - 1.0- 0.71- 0.6
-000044f0: 5d2c 3132 3733 2e31 352c 3133 3438 2e31  ],1273.15,1348.1
-00004500: 352c 3133 3733 2e31 352c 3133 3630 2c32  5,1373.15,1360,2
-00004510: 2e37 3233 322c 440d 0a35 3731 382c 442c  .7232,D..5718,D,
-00004520: 3730 3237 2c79 6573 2c79 6573 2c79 6573  7027,yes,yes,yes
-00004530: 2c79 6573 2c2c 7965 732c 7965 732c 7965  ,yes,,yes,yes,ye
-00004540: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00004550: 6e65 2c64 6965 7365 6c2c 3131 302c 3338  ne,diesel,110,38
-00004560: 302c 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c  0,front,,,,,,,,,
-00004570: 2c2c 312e 3438 2c34 2e38 2c32 2e37 352c  ,,1.48,4.8,2.75,
-00004580: 312e 3834 2c2c 3231 3931 2c70 6172 7469  1.84,,2191,parti
-00004590: 636c 6520 6669 6c74 6572 2c34 2c64 6f68  cle filter,4,doh
-000045a0: 632c 636f 6d6d 6f6e 2072 6169 6c2c 3632  c,common rail,62
-000045b0: 2c34 3530 302c 3131 302c 3230 3030 2c33  ,4500,110,2000,3
-000045c0: 3830 2c79 6573 2c34 2c73 7461 7469 6f6e  80,yes,4,station
-000045d0: 7761 676f 6e2c 352c 6176 6169 6c61 626c  wagon,5,availabl
-000045e0: 652c 3336 3939 302c 352c 3230 3135 2c6d  e,36990,5,2015,m
-000045f0: 616e 7561 6c2c 392e 322c 342e 322c 3131  anual,9.2,4.2,11
-00004600: 302c 422c 332e 372c 3231 302c 352e 312c  0,B,3.7,210,5.1,
-00004610: 322e 3831 2c31 3935 302c 3133 3935 2c32  2.81,1950,1395,2
-00004620: 3039 302c 2c39 342e 332c 3331 322e 3432  090,,94.3,312.42
-00004630: 352c 3332 392e 3735 3732 3831 362c 5b33  5,329.7572816,[3
-00004640: 2e35 342d 2031 2e38 332d 2031 2e35 372d  .54- 1.83- 1.57-
-00004650: 2031 2e31 352d 2030 2e38 392d 2030 2e37   1.15- 0.89- 0.7
-00004660: 355d 2c31 3335 332e 3135 2c31 3432 382e  5],1353.15,1428.
-00004670: 3135 2c31 3435 332e 3135 2c31 3437 302c  15,1453.15,1470,
-00004680: 322e 3732 3332 2c44 0d0a 3336 3539 312c  2.7232,D..36591,
-00004690: 442c 3531 3937 302c 7965 732c 7965 732c  D,51970,yes,yes,
-000046a0: 7965 732c 7965 732c 2c6e 6f2c 6e6f 2c79  yes,yes,,no,no,y
-000046b0: 6573 2c6e 6f2c 2c66 7565 6c20 656e 6769  es,no,,fuel engi
-000046c0: 6e65 2c70 6574 726f 6c2c 3130 382c 3139  ne,petrol,108,19
-000046d0: 362c 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c  6,front,,,,,,,,,
-000046e0: 2c2c 312e 3532 352c 342e 3731 352c 322e  ,,1.525,4.715,2.
-000046f0: 372c 312e 3736 2c2c 3139 3938 2c72 6567  7,1.76,,1998,reg
-00004700: 756c 6172 2c34 2c64 6f68 632c 6469 7265  ular,4,dohc,dire
-00004710: 6374 2069 6e6a 6563 7469 6f6e 2c36 302c  ct injection,60,
-00004720: 3537 3030 2c31 3038 2c34 3030 302c 3139  5700,108,4000,19
-00004730: 362c 6e6f 2c34 2c73 7461 7469 6f6e 7761  6,no,4,stationwa
-00004740: 676f 6e2c 352c 3230 3038 2c33 3139 3035  gon,5,2008,31905
-00004750: 2c35 2c32 3030 362c 6d61 6e75 616c 2c39  ,5,2006,manual,9
-00004760: 2e36 2c38 2e31 2c31 3933 2c47 2c36 2e36  .6,8.1,193,G,6.6
-00004770: 2c32 3130 2c31 302e 372c 332e 3638 2c32  ,210,10.7,3.68,2
-00004780: 3935 302c 3133 3430 2c31 3839 352c 3930  950,1340,1895,90
-00004790: 2c38 362c 3239 392e 3735 2c33 3133 2e39  ,86,299.75,313.9
-000047a0: 3830 3538 3235 2c5b 332e 3534 2d20 322e  805825,[3.54- 2.
-000047b0: 3035 2d20 312e 3333 2d20 312e 3033 2d20  05- 1.33- 1.03- 
-000047c0: 302e 3832 5d2c 3132 3939 2e35 2c31 3337  0.82],1299.5,137
-000047d0: 342e 352c 3133 3939 2e35 2c31 3336 302c  4.5,1399.5,1360,
-000047e0: 322e 3638 342c 440d 0a34 3335 302c 442c  2.684,D..4350,D,
-000047f0: 3534 3132 2c79 6573 2c79 6573 2c79 6573  5412,yes,yes,yes
-00004800: 2c6e 6f2c 2c6e 6f2c 6e6f 2c79 6573 2c6e  ,no,,no,no,yes,n
-00004810: 6f2c 2c66 7565 6c20 656e 6769 6e65 2c64  o,,fuel engine,d
-00004820: 6965 7365 6c2c 3835 2c32 3830 2c66 726f  iesel,85,280,fro
-00004830: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35  nt,,,,,,,,,,,1.5
-00004840: 3235 2c34 2e37 2c32 2e37 2c31 2e37 362c  25,4.7,2.7,1.76,
-00004850: 2c31 3939 352c 6e6f 2c34 2c64 6f68 632c  ,1995,no,4,dohc,
-00004860: 636f 6d6d 6f6e 2072 6169 6c2c 3630 2c34  common rail,60,4
-00004870: 3030 302c 3835 2c32 3030 302c 3238 302c  000,85,2000,280,
-00004880: 7965 732c 342c 7374 6174 696f 6e77 6167  yes,4,stationwag
-00004890: 6f6e 2c35 2c32 3030 362c 3330 3230 302c  on,5,2006,30200,
-000048a0: 352c 3230 3033 2c6d 616e 7561 6c2c 3131  5,2003,manual,11
-000048b0: 2e34 2c36 2c31 3538 2c47 2c35 2e31 2c31  .4,6,158,G,5.1,1
-000048c0: 3935 2c37 2e37 2c33 2e36 382c 3235 3530  95,7.7,3.68,2550
-000048d0: 2c31 3430 352c 3139 3730 2c39 302c 3934  ,1405,1970,90,94
-000048e0: 2c32 3931 2e31 3435 2c33 3036 2e37 3437  ,291.145,306.747
-000048f0: 3537 3238 2c5b 332e 3534 2d20 312e 3931  5728,[3.54- 1.91
-00004900: 2d20 312e 3236 2d20 302e 3932 2d20 302e  - 1.26- 0.92- 0.
-00004910: 3639 5d2c 3133 3634 2e35 2c31 3433 392e  69],1364.5,1439.
-00004920: 352c 3134 3634 2e35 2c31 3437 302c 322e  5,1464.5,1470,2.
-00004930: 3638 342c 440d 0a33 3933 3936 2c45 2c35  684,D..39396,E,5
-00004940: 3630 3235 2c79 6573 2c79 6573 2c79 6573  6025,yes,yes,yes
-00004950: 2c79 6573 2c2c 3834 332c 7965 732c 7965  ,yes,,843,yes,ye
-00004960: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00004970: 6e65 2c70 6574 726f 6c2c 3232 352c 3430  ne,petrol,225,40
-00004980: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00004990: 2c2c 2c2c 2c2c 2c31 2e34 3634 2c34 2e39  ,,,,,,,1.464,4.9
-000049a0: 3037 2c32 2e39 3638 2c31 2e38 362c 2c32  07,2.968,1.86,,2
-000049b0: 3937 392c 7265 6775 6c61 722c 362c 646f  979,regular,6,do
-000049c0: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-000049d0: 696f 6e2c 3730 2c35 3830 302c 3232 352c  ion,70,5800,225,
-000049e0: 3132 3030 2c34 3030 2c79 6573 2c34 2c73  1200,400,yes,4,s
-000049f0: 6564 616e 2c34 2c61 7661 696c 6162 6c65  edan,4,available
-00004a00: 2c37 3032 3031 2c35 2c32 3031 332c 6175  ,70201,5,2013,au
-00004a10: 746f 6d61 7469 632c 352e 362c 372e 362c  tomatic,5.6,7.6,
-00004a20: 3137 382c 442c 352e 392c 3235 302c 3130  178,D,5.9,250,10
-00004a30: 2e35 2c33 2e30 382c 3139 3530 2c31 3734  .5,3.08,1950,174
-00004a40: 302c 3233 3635 2c31 3030 2c38 392e 362c  0,2365,100,89.6,
-00004a50: 3331 322e 3432 352c 3332 392e 3735 3732  312.425,329.7572
-00004a60: 3831 362c 5b34 2e37 312d 2033 2e31 342d  816,[4.71- 3.14-
-00004a70: 2032 2e31 312d 2031 2e36 372d 2031 2e32   2.11- 1.67- 1.2
-00004a80: 392d 2031 2e30 2d20 302e 3834 2d20 302e  9- 1.0- 0.84- 0.
-00004a90: 3637 5d2c 3136 3932 2e37 352c 3137 3637  67],1692.75,1767
-00004aa0: 2e37 352c 3137 3932 2e37 352c 3138 3130  .75,1792.75,1810
-00004ab0: 2c32 2e37 3233 3034 2c45 0d0a 3430 3539  ,2.72304,E..4059
-00004ac0: 352c 452c 3537 3732 362c 7965 732c 7965  5,E,57726,yes,ye
-00004ad0: 732c 7965 732c 7965 732c 2c38 3433 2c79  s,yes,yes,,843,y
-00004ae0: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
-00004af0: 2065 6e67 696e 652c 6469 6573 656c 2c31   engine,diesel,1
-00004b00: 3130 2c33 3630 2c72 6561 722c 2c2c 2c2c  10,360,rear,,,,,
-00004b10: 2c2c 2c2c 2c2c 312e 3436 342c 342e 3930  ,,,,,,1.464,4.90
-00004b20: 372c 322e 3936 382c 312e 3836 2c2c 3139  7,2.968,1.86,,19
-00004b30: 3935 2c70 6172 7469 636c 6520 6669 6c74  95,particle filt
-00004b40: 6572 2c34 2c64 6f68 632c 636f 6d6d 6f6e  er,4,dohc,common
-00004b50: 2072 6169 6c2c 3730 2c34 3030 302c 3131   rail,70,4000,11
-00004b60: 302c 3137 3530 2c33 3630 2c79 6573 2c34  0,1750,360,yes,4
-00004b70: 2c73 6564 616e 2c34 2c61 7661 696c 6162  ,sedan,4,availab
-00004b80: 6c65 2c34 3839 3835 2c35 2c32 3031 342c  le,48985,5,2014,
-00004b90: 6d61 6e75 616c 2c39 2e35 2c34 2e33 2c31  manual,9.5,4.3,1
-00004ba0: 3134 2c42 2c33 2e39 2c32 3138 2c35 2e31  14,B,3.9,218,5.1
-00004bb0: 2c33 2e32 332c 3230 3030 2c31 3539 302c  ,3.23,2000,1590,
-00004bc0: 3232 3235 2c31 3030 2c39 302c 3331 322e  2225,100,90,312.
-00004bd0: 3432 352c 3332 392e 3735 3732 3831 362c  425,329.7572816,
-00004be0: 5b34 2e31 312d 2032 2e32 352d 2031 2e34  [4.11- 2.25- 1.4
-00004bf0: 2d20 312e 302d 2030 2e38 2d20 302e 3636  - 1.0- 0.8- 0.66
-00004c00: 5d2c 3135 3432 2e37 352c 3136 3137 2e37  ],1542.75,1617.7
-00004c10: 352c 3136 3432 2e37 352c 3135 3930 2c32  5,1642.75,1590,2
-00004c20: 2e37 3233 3034 2c45 0d0a 3539 3039 2c45  .72304,E..5909,E
-00004c30: 2c37 3236 322c 7965 732c 7965 732c 7965  ,7262,yes,yes,ye
-00004c40: 732c 7965 732c 2c6e 6f2c 7965 732c 7965  s,yes,,no,yes,ye
-00004c50: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00004c60: 6e65 2c70 6574 726f 6c2c 3234 352c 3434  ne,petrol,245,44
-00004c70: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00004c80: 2c2c 2c2c 2c2c 2c31 2e34 3535 2c34 2e39  ,,,,,,,1.455,4.9
-00004c90: 3333 2c32 2e39 3132 2c31 2e38 3734 2c2c  33,2.912,1.874,,
-00004ca0: 3239 3935 2c72 6567 756c 6172 2c36 2c64  2995,regular,6,d
-00004cb0: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
-00004cc0: 7469 6f6e 2c37 352c 3535 3030 2c32 3435  tion,75,5500,245
-00004cd0: 2c32 3930 302c 3434 302c 7965 732c 342c  ,2900,440,yes,4,
-00004ce0: 7365 6461 6e2c 342c 6176 6169 6c61 626c  sedan,4,availabl
-00004cf0: 652c 3734 3638 302c 352c 3230 3134 2c61  e,74680,5,2014,a
-00004d00: 7574 6f6d 6174 6963 2c35 2e31 2c37 2e34  utomatic,5.1,7.4
-00004d10: 2c31 3732 2c43 2c36 2c32 3530 2c39 2e38  ,172,C,6,250,9.8
-00004d20: 2c34 2e30 392c 3230 3030 2c31 3732 352c  ,4.09,2000,1725,
-00004d30: 3233 3630 2c31 3030 2c38 392c 3331 342e  2360,100,89,314.
-00004d40: 3539 352c 3332 382e 3938 3035 3832 352c  595,328.9805825,
-00004d50: 5b33 2e36 392d 2032 2e31 352d 2031 2e34  [3.69- 2.15- 1.4
-00004d60: 312d 2031 2e30 332d 2030 2e37 392d 2030  1- 1.03- 0.79- 0
-00004d70: 2e36 332d 2030 2e35 325d 2c31 3637 342e  .63- 0.52],1674.
-00004d80: 3337 352c 3137 3439 2e33 3735 2c31 3737  375,1749.375,177
-00004d90: 342e 3337 352c 3137 3030 2c32 2e37 3236  4.375,1700,2.726
-00004da0: 3637 2c45 0d0a 3538 3937 2c45 2c37 3235  67,E..5897,E,725
-00004db0: 302c 7965 732c 7965 732c 7965 732c 7965  0,yes,yes,yes,ye
-00004dc0: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
-00004dd0: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
-00004de0: 6965 7365 6c2c 3136 302c 3530 302c 6672  iesel,160,500,fr
-00004df0: 6f6e 742b 7265 6172 2c2c 2c2c 2c2c 2c2c  ont+rear,,,,,,,,
-00004e00: 2c2c 2c31 2e34 3535 2c34 2e39 3333 2c32  ,,,1.455,4.933,2
-00004e10: 2e39 3132 2c31 2e38 3734 2c2c 3239 3637  .912,1.874,,2967
-00004e20: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
-00004e30: 2c36 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,6,dohc,common r
-00004e40: 6169 6c2c 3733 2c33 3235 302c 3136 302c  ail,73,3250,160,
-00004e50: 3132 3530 2c35 3030 2c79 6573 2c34 2c73  1250,500,yes,4,s
-00004e60: 6564 616e 2c34 2c61 7661 696c 6162 6c65  edan,4,available
-00004e70: 2c37 3039 3730 2c35 2c32 3031 342c 6175  ,70970,5,2014,au
-00004e80: 746f 6d61 7469 632c 362e 362c 352e 312c  tomatic,6.6,5.1,
-00004e90: 3133 332c 432c 342e 362c 3234 342c 352e  133,C,4.6,244,5.
-00004ea0: 392c 342e 3039 2c31 3735 302c 3137 3430  9,4.09,1750,1740
-00004eb0: 2c32 3337 352c 3130 302c 3931 2e34 2c33  ,2375,100,91.4,3
-00004ec0: 3230 2e38 362c 3333 332e 3330 3039 3730  20.86,333.300970
-00004ed0: 392c 5b33 2e36 392d 2032 2e31 352d 2031  9,[3.69- 2.15- 1
-00004ee0: 2e33 342d 2030 2e39 372d 2030 2e37 342d  .34- 0.97- 0.74-
-00004ef0: 2030 2e35 372d 2030 2e34 365d 2c31 3639   0.57- 0.46],169
-00004f00: 302e 3732 352c 3137 3635 2e37 3235 2c31  0.725,1765.725,1
-00004f10: 3739 302e 3732 352c 3138 3130 2c32 2e37  790.725,1810,2.7
-00004f20: 3236 3637 2c45 0d0a 3539 3238 2c45 2c37  2667,E..5928,E,7
-00004f30: 3238 352c 7965 732c 7965 732c 7965 732c  285,yes,yes,yes,
-00004f40: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-00004f50: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-00004f60: 2c70 6574 726f 6c2c 3234 352c 3434 302c  ,petrol,245,440,
-00004f70: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
-00004f80: 2c2c 2c2c 2c31 2e34 322c 342e 3937 342c  ,,,,,1.42,4.974,
-00004f90: 322e 3931 342c 312e 3931 312c 2c32 3939  2.914,1.911,,299
-00004fa0: 352c 7265 6775 6c61 722c 362c 646f 6863  5,regular,6,dohc
-00004fb0: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
-00004fc0: 6e2c 3635 2c35 3330 302c 3234 352c 3239  n,65,5300,245,29
-00004fd0: 3030 2c34 3430 2c79 6573 2c34 2c68 6174  00,440,yes,4,hat
-00004fe0: 6368 6261 636b 2c35 2c61 7661 696c 6162  chback,5,availab
-00004ff0: 6c65 2c38 3330 3930 2c34 2c32 3031 342c  le,83090,4,2014,
-00005000: 6175 746f 6d61 7469 632c 352e 332c 372e  automatic,5.3,7.
-00005010: 362c 3137 362c 432c 362e 322c 3235 302c  6,176,C,6.2,250,
-00005020: 3130 2c34 2e30 392c 3139 3530 2c31 3738  10,4.09,1950,178
-00005030: 352c 3234 3230 2c31 3030 2c38 392c 3331  5,2420,100,89,31
-00005040: 382e 3130 352c 3333 332e 3334 3935 3134  8.105,333.349514
-00005050: 362c 5b33 2e36 392d 2032 2e31 352d 2031  6,[3.69- 2.15- 1
-00005060: 2e34 312d 2031 2e30 332d 2030 2e37 392d  .41- 1.03- 0.79-
-00005070: 2030 2e36 332d 2030 2e35 325d 2c31 3734   0.63- 0.52],174
-00005080: 312e 3132 352c 3138 3136 2e31 3235 2c31  1.125,1816.125,1
-00005090: 3834 312e 3132 352c 3138 3130 2c32 2e37  841.125,1810,2.7
-000050a0: 3133 3632 2c45 0d0a 3539 3135 2c45 2c37  1362,E..5915,E,7
-000050b0: 3237 322c 7965 732c 7965 732c 7965 732c  272,yes,yes,yes,
-000050c0: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
-000050d0: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-000050e0: 2c64 6965 7365 6c2c 3230 302c 3538 302c  ,diesel,200,580,
-000050f0: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
-00005100: 2c2c 2c2c 2c31 2e34 322c 342e 3937 342c  ,,,,,1.42,4.974,
-00005110: 322e 3931 342c 312e 3931 312c 2c32 3936  2.914,1.911,,296
-00005120: 372c 7061 7274 6963 6c65 2066 696c 7465  7,particle filte
-00005130: 722c 362c 646f 6863 2c63 6f6d 6d6f 6e20  r,6,dohc,common 
-00005140: 7261 696c 2c36 352c 3335 3030 2c32 3030  rail,65,3500,200
-00005150: 2c31 3530 302c 3538 302c 7965 732c 342c  ,1500,580,yes,4,
-00005160: 6861 7463 6862 6163 6b2c 352c 6176 6169  hatchback,5,avai
-00005170: 6c61 626c 652c 3738 3539 302c 342c 3230  lable,78590,4,20
-00005180: 3134 2c61 7574 6f6d 6174 6963 2c35 2e37  14,automatic,5.7
-00005190: 2c35 2e32 2c31 3336 2c42 2c34 2e37 2c32  ,5.2,136,B,4.7,2
-000051a0: 3530 2c36 2c33 2e38 382c 3136 3530 2c31  50,6,3.88,1650,1
-000051b0: 3830 352c 3234 3430 2c31 3030 2c39 312e  805,2440,100,91.
-000051c0: 342c 3331 382e 3130 352c 3333 332e 3334  4,318.105,333.34
-000051d0: 3935 3134 362c 5b33 2e36 392d 2032 2e31  95146,[3.69- 2.1
-000051e0: 352d 2031 2e33 342d 2030 2e39 372d 2030  5- 1.34- 0.97- 0
-000051f0: 2e37 342d 2030 2e35 372d 2030 2e34 365d  .74- 0.57- 0.46]
-00005200: 2c31 3736 312e 3132 352c 3138 3336 2e31  ,1761.125,1836.1
-00005210: 3235 2c31 3836 312e 3132 352c 3138 3130  25,1861.125,1810
-00005220: 2c32 2e37 3133 3632 2c45 0d0a 3430 3133  ,2.71362,E..4013
-00005230: 302c 452c 3537 3038 342c 7965 732c 7965  0,E,57084,yes,ye
-00005240: 732c 7965 732c 7965 732c 2c6e 6f2c 3131  s,yes,yes,,no,11
-00005250: 3435 2c79 6573 2c79 6573 2c2c 6675 656c  45,yes,yes,,fuel
-00005260: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
-00005270: 3335 2c32 3730 2c72 6561 722c 2c2c 2c2c  35,270,rear,,,,,
-00005280: 2c2c 2c2c 2c2c 312e 3531 322c 342e 3839  ,,,,,,1.512,4.89
-00005290: 352c 322e 3837 342c 312e 3835 342c 2c31  5,2.874,1.854,,1
-000052a0: 3739 362c 7265 6775 6c61 722c 342c 646f  796,regular,4,do
-000052b0: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-000052c0: 696f 6e2c 3539 2c35 3235 302c 3133 352c  ion,59,5250,135,
-000052d0: 3138 3030 2c32 3730 2c79 6573 2c34 2c73  1800,270,yes,4,s
-000052e0: 7461 7469 6f6e 7761 676f 6e2c 352c 3230  tationwagon,5,20
-000052f0: 3133 2c35 3431 3534 2c35 2c32 3031 312c  13,54154,5,2011,
-00005300: 6d61 6e75 616c 2c38 2e37 2c37 2e35 2c31  manual,8.7,7.5,1
-00005310: 3735 2c44 2c36 2e31 2c32 3235 2c31 302c  75,D,6.1,225,10,
-00005320: 332e 3037 2c32 3435 302c 3136 3335 2c32  3.07,2450,1635,2
-00005330: 3331 302c 3130 302c 3835 2c33 3031 2e38  310,100,85,301.8
-00005340: 3935 2c33 3136 2e36 3530 3438 3534 2c5b  95,316.6504854,[
-00005350: 342e 3939 2d20 322e 3832 2d20 312e 3738  4.99- 2.82- 1.78
-00005360: 2d20 312e 3235 2d20 312e 302d 2030 2e38  - 1.25- 1.0- 0.8
-00005370: 325d 2c31 3539 352e 3137 352c 3136 3730  2],1595.175,1670
-00005380: 2e31 3735 2c31 3639 352e 3137 352c 3137  .175,1695.175,17
-00005390: 3030 2c32 2e38 3033 3234 382c 450d 0a34  00,2.803248,E..4
-000053a0: 3233 3633 2c45 2c36 3032 3434 2c79 6573  2363,E,60244,yes
-000053b0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-000053c0: 2c31 3134 352c 7965 732c 7965 732c 2c66  ,1145,yes,yes,,f
-000053d0: 7565 6c20 656e 6769 6e65 2c64 6965 7365  uel engine,diese
-000053e0: 6c2c 3137 302c 3530 302c 7265 6172 2c2c  l,170,500,rear,,
-000053f0: 2c2c 2c2c 2c2c 2c2c 2c31 2e35 3132 2c34  ,,,,,,,,,1.512,4
-00005400: 2e38 3935 2c32 2e38 3734 2c31 2e38 3534  .895,2.874,1.854
-00005410: 2c2c 3231 3433 2c70 6172 7469 636c 6520  ,,2143,particle 
-00005420: 6669 6c74 6572 2c34 2c64 6f68 632c 636f  filter,4,dohc,co
-00005430: 6d6d 6f6e 2072 6169 6c2c 3539 2c34 3230  mmon rail,59,420
-00005440: 302c 3135 302c 3136 3030 2c35 3030 2c79  0,150,1600,500,y
-00005450: 6573 2c34 2c73 7461 7469 6f6e 7761 676f  es,4,stationwago
-00005460: 6e2c 352c 3230 3133 2c36 3238 3034 2c35  n,5,2013,62804,5
-00005470: 2c32 3031 322c 6175 746f 6d61 7469 632c  ,2012,automatic,
-00005480: 372e 382c 342e 342c 3131 362c 422c 342e  7.8,4.4,116,B,4.
-00005490: 342c 3233 322c 342e 352c 322e 3635 2c31  4,232,4.5,2.65,1
-000054a0: 3930 302c 3138 3535 2c32 3535 352c 3130  900,1855,2555,10
-000054b0: 302c 3939 2c33 3031 2e38 3935 2c33 3136  0,99,301.895,316
-000054c0: 2e36 3530 3438 3534 2c5b 342e 3338 2d20  .6504854,[4.38- 
-000054d0: 322e 3836 2d20 312e 3932 2d20 312e 3337  2.86- 1.92- 1.37
-000054e0: 2d20 312e 302d 2030 2e38 322d 2030 2e37  - 1.0- 0.82- 0.7
-000054f0: 335d 2c31 3831 352e 3137 352c 3138 3930  3],1815.175,1890
-00005500: 2e31 3735 2c31 3931 352e 3137 352c 3139  .175,1915.175,19
-00005510: 3330 2c32 2e38 3033 3234 382c 450d 0a33  30,2.803248,E..3
-00005520: 3437 3630 2c45 2c34 3932 3431 2c79 6573  4760,E,49241,yes
-00005530: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-00005540: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-00005550: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
-00005560: 2c39 322c 3230 302c 6672 6f6e 742c 2c2c  ,92,200,front,,,
-00005570: 2c2c 2c2c 2c2c 2c2c 312e 3531 2c34 2e38  ,,,,,,,,1.51,4.8
-00005580: 3333 2c32 2e37 3631 2c31 2e38 3137 2c2c  33,2.761,1.817,,
-00005590: 3133 3930 2c72 6567 756c 6172 2c34 2c64  1390,regular,4,d
-000055a0: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
-000055b0: 7469 6f6e 2c36 302c 3530 3030 2c39 322c  tion,60,5000,92,
-000055c0: 3135 3030 2c32 3030 2c79 6573 2c34 2c73  1500,200,yes,4,s
-000055d0: 7461 7469 6f6e 7761 676f 6e2c 352c 6176  tationwagon,5,av
-000055e0: 6169 6c61 626c 652c 3333 3033 302c 352c  ailable,33030,5,
-000055f0: 3230 3134 2c6d 616e 7561 6c2c 3130 2e36  2014,manual,10.6
-00005600: 2c36 2e31 2c31 3432 2c42 2c35 2c32 3033  ,6.1,142,B,5,203
-00005610: 2c38 2c34 2e30 362c 3236 3530 2c31 3338  ,8,4.06,2650,138
-00005620: 392c 3230 3532 2c31 3030 2c37 352e 362c  9,2052,100,75.6,
-00005630: 3239 312e 3134 352c 3330 362e 3734 3735  291.145,306.7475
-00005640: 3732 382c 5b33 2e36 322d 2031 2e39 352d  728,[3.62- 1.95-
-00005650: 2031 2e32 382d 2030 2e39 372d 2030 2e37   1.28- 0.97- 0.7
-00005660: 382d 2030 2e36 355d 2c31 3334 382e 352c  8- 0.65],1348.5,
-00005670: 3134 3233 2e35 2c31 3434 382e 352c 3133  1423.5,1448.5,13
-00005680: 3630 2c32 2e37 3433 3637 2c45 0d0a 3334  60,2.74367,E..34
-00005690: 3736 362c 452c 3439 3234 372c 7965 732c  766,E,49247,yes,
-000056a0: 7965 732c 7965 732c 7965 732c 2c6e 6f2c  yes,yes,yes,,no,
-000056b0: 7965 732c 7965 732c 7965 732c 2c66 7565  yes,yes,yes,,fue
-000056c0: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
-000056d0: 3737 2c32 3530 2c66 726f 6e74 2c2c 2c2c  77,250,front,,,,
-000056e0: 2c2c 2c2c 2c2c 2c31 2e35 312c 342e 3833  ,,,,,,,1.51,4.83
-000056f0: 332c 322e 3736 312c 312e 3831 372c 2c31  3,2.761,1.817,,1
-00005700: 3539 382c 7061 7274 6963 6c65 2066 696c  598,particle fil
-00005710: 7465 722c 342c 646f 6863 2c63 6f6d 6d6f  ter,4,dohc,commo
-00005720: 6e20 7261 696c 2c36 302c 3434 3030 2c37  n rail,60,4400,7
-00005730: 372c 3135 3030 2c32 3530 2c79 6573 2c34  7,1500,250,yes,4
-00005740: 2c73 7461 7469 6f6e 7761 676f 6e2c 352c  ,stationwagon,5,
-00005750: 6176 6169 6c61 626c 652c 3333 3536 302c  available,33560,
-00005760: 352c 3230 3134 2c6d 616e 7561 6c2c 3132  5,2014,manual,12
-00005770: 2e33 2c34 2e33 2c31 3130 2c42 2c33 2e36  .3,4.3,110,B,3.6
-00005780: 2c31 3935 2c35 2e32 2c33 2e33 392c 3230  ,195,5.2,3.39,20
-00005790: 3030 2c31 3434 312c 3231 3034 2c31 3030  00,1441,2104,100
-000057a0: 2c38 302e 352c 3239 312e 3134 352c 3330  ,80.5,291.145,30
-000057b0: 362e 3734 3735 3732 382c 5b34 2e31 312d  6.7475728,[4.11-
-000057c0: 2032 2e31 322d 2031 2e33 362d 2030 2e39   2.12- 1.36- 0.9
-000057d0: 372d 2030 2e37 332d 2030 2e35 395d 2c31  7- 0.73- 0.59],1
-000057e0: 3430 302e 352c 3134 3735 2e35 2c31 3530  400.5,1475.5,150
-000057f0: 302e 352c 3134 3730 2c32 2e37 3433 3637  0.5,1470,2.74367
-00005800: 2c45 0d0a 3138 3335 2c45 2c32 3739 372c  ,E..1835,E,2797,
-00005810: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
-00005820: 2c6e 6f2c 7965 732c 7965 732c 7965 732c  ,no,yes,yes,yes,
-00005830: 2c66 7565 6c20 656e 6769 6e65 2c64 6965  ,fuel engine,die
-00005840: 7365 6c2c 3135 382c 3432 302c 6672 6f6e  sel,158,420,fron
-00005850: 742c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3439  t,,,,,,,,,,,1.49
-00005860: 332c 342e 3835 312c 322e 3833 352c 312e  3,4.851,2.835,1.
-00005870: 3836 2c2c 3234 3030 2c70 6172 7469 636c  86,,2400,particl
-00005880: 6520 6669 6c74 6572 2c35 2c64 6f68 632c  e filter,5,dohc,
-00005890: 636f 6d6d 6f6e 2072 6169 6c2c 3730 2c34  common rail,70,4
-000058a0: 3030 302c 3135 382c 3134 3030 2c34 3230  000,158,1400,420
-000058b0: 2c79 6573 2c34 2c73 6564 616e 2c34 2c32  ,yes,4,sedan,4,2
-000058c0: 3031 342c 3533 3939 352c 352c 3230 3133  014,53995,5,2013
-000058d0: 2c6d 616e 7561 6c2c 372e 362c 342e 362c  ,manual,7.6,4.6,
-000058e0: 3132 302c 422c 342c 3233 302c 352e 362c  120,B,4,230,5.6,
-000058f0: 332e 3737 2c31 3935 302c 3135 3335 2c32  3.77,1950,1535,2
-00005900: 3139 302c 3130 302c 3933 2e31 352c 3330  190,100,93.15,30
-00005910: 332e 3635 2c33 3138 2e38 3334 3935 3135  3.65,318.8349515
-00005920: 2c5b 332e 3339 2d20 312e 3931 2d20 312e  ,[3.39- 1.91- 1.
-00005930: 3139 2d20 302e 3834 2d20 302e 3635 2d20  19- 0.84- 0.65- 
-00005940: 302e 3534 5d2c 3134 3837 2e37 352c 3135  0.54],1487.75,15
-00005950: 3632 2e37 352c 3135 3837 2e37 352c 3135  62.75,1587.75,15
-00005960: 3930 2c32 2e37 3736 3938 2c45 0d0a 3336  90,2.77698,E..36
-00005970: 3130 312c 452c 3531 3237 332c 6e6f 2c79  101,E,51273,no,y
-00005980: 6573 2c6e 6f2c 6e6f 2c2c 6e6f 2c6e 6f2c  es,no,no,,no,no,
-00005990: 7965 732c 6e6f 2c2c 6675 656c 2065 6e67  yes,no,,fuel eng
-000059a0: 696e 652c 7065 7472 6f6c 2c31 3134 2c31  ine,petrol,114,1
-000059b0: 3831 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  81,front,,,,,,,,
-000059c0: 2c2c 2c31 2e34 3333 2c34 2e36 3035 2c32  ,,,1.433,4.605,2
-000059d0: 2e36 362c 312e 3735 322c 2c31 3939 352c  .66,1.752,,1995,
-000059e0: 7265 6775 6c61 722c 342c 646f 6863 2c6d  regular,4,dohc,m
-000059f0: 756c 7469 706f 696e 7420 696e 6a65 6374  ultipoint inject
-00005a00: 696f 6e2c 3635 2c36 3530 302c 3131 342c  ion,65,6500,114,
-00005a10: 3335 3030 2c31 3831 2c6e 6f2c 342c 7365  3500,181,no,4,se
-00005a20: 6461 6e2c 342c 3139 3935 2c33 3535 3939  dan,4,1995,35599
-00005a30: 2c35 2c31 3939 342c 6175 746f 6d61 7469  ,5,1994,automati
-00005a40: 632c 3133 2e39 2c39 2e32 2c2c 2c2c 3230  c,13.9,9.2,,,,20
-00005a50: 342c 2c33 2e33 352c 3236 3530 2c31 3330  4,,3.35,2650,130
-00005a60: 302c 3138 3030 2c35 302c 3930 2c32 3731  0,1800,50,90,271
-00005a70: 2e35 3935 2c32 3839 2e33 3638 3933 322c  .595,289.368932,
-00005a80: 5b32 2e35 382d 2031 2e34 312d 2031 2e30  [2.58- 1.41- 1.0
-00005a90: 2d20 302e 3734 5d2c 3132 3536 2e31 3235  - 0.74],1256.125
-00005aa0: 2c31 3333 312e 3132 352c 3133 3536 2e31  ,1331.125,1356.1
-00005ab0: 3235 2c31 3336 302c 322e 3531 3036 3136  25,1360,2.510616
-00005ac0: 2c45 0d0a 3432 3838 362c 452c 3630 3939  ,E..42886,E,6099
-00005ad0: 332c 6e6f 2c79 6573 2c6e 6f2c 6e6f 2c2c  3,no,yes,no,no,,
-00005ae0: 6e6f 2c6e 6f2c 7965 732c 6e6f 2c2c 6675  no,no,yes,no,,fu
-00005af0: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
-00005b00: 2c38 372c 3234 352c 6672 6f6e 742c 2c2c  ,87,245,front,,,
-00005b10: 2c2c 2c2c 2c2c 2c2c 312e 3433 332c 342e  ,,,,,,,,1.433,4.
-00005b20: 3630 352c 322e 3636 2c31 2e37 3532 2c2c  605,2.66,1.752,,
-00005b30: 3235 3030 2c6e 6f2c 342c 6f68 632c 696e  2500,no,4,ohc,in
-00005b40: 6469 7265 6374 2069 6e6a 6563 7469 6f6e  direct injection
-00005b50: 2c36 352c 3431 3030 2c38 372c 3234 3030  ,65,4100,87,2400
-00005b60: 2c32 3435 2c79 6573 2c32 2c73 6564 616e  ,245,yes,2,sedan
-00005b70: 2c34 2c31 3939 352c 3338 3638 352c 352c  ,4,1995,38685,5,
-00005b80: 3139 3932 2c6d 616e 7561 6c2c 3131 2e35  1992,manual,11.5
-00005b90: 2c37 2e32 2c2c 2c2c 3139 322c 2c33 2e35  ,7.2,,,,192,,3.5
-00005ba0: 362c 3236 3530 2c31 3332 362c 3138 3235  6,2650,1326,1825
-00005bb0: 2c35 302c 3932 2c32 3831 2e37 362c 3239  ,50,92,281.76,29
-00005bc0: 382e 3534 3336 3839 332c 5b33 2e37 352d  8.5436893,[3.75-
-00005bd0: 2032 2e31 382d 2031 2e33 382d 2030 2e39   2.18- 1.38- 0.9
-00005be0: 382d 2030 2e37 325d 2c31 3238 322e 3132  8- 0.72],1282.12
-00005bf0: 352c 3133 3537 2e31 3235 2c31 3338 322e  5,1357.125,1382.
-00005c00: 3132 352c 3133 3630 2c32 2e35 3130 3631  125,1360,2.51061
-00005c10: 362c 450d 0a31 3433 312c 452c 3137 3830  6,E..1431,E,1780
-00005c20: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00005c30: 2c2c 7965 732c 6e6f 2c79 6573 2c6e 6f2c  ,,yes,no,yes,no,
-00005c40: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
-00005c50: 726f 6c2c 3138 332c 3331 302c 7265 6172  rol,183,310,rear
-00005c60: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 332c  ,,,,,,,,,,,1.43,
-00005c70: 342e 3832 352c 322e 3835 2c31 2e38 3135  4.825,2.85,1.815
-00005c80: 2c2c 3239 3935 2c72 6567 756c 6172 2c36  ,,2995,regular,6
-00005c90: 2c64 6f68 632c 6469 7265 6374 2069 6e6a  ,dohc,direct inj
-00005ca0: 6563 7469 6f6e 2c37 312c 3632 3030 2c31  ection,71,6200,1
-00005cb0: 3833 2c33 3530 302c 3331 302c 6e6f 2c34  83,3500,310,no,4
-00005cc0: 2c73 6564 616e 2c34 2c32 3031 302c 3635  ,sedan,4,2010,65
-00005cd0: 3430 352c 352c 3230 3038 2c61 7574 6f6d  405,5,2008,autom
-00005ce0: 6174 6963 2c37 2e32 2c39 2e35 2c32 3234  atic,7.2,9.5,224
-00005cf0: 2c47 2c37 2c32 3430 2c31 342c 332e 3733  ,G,7,240,14,3.73
-00005d00: 2c2c 3135 3935 2c32 3132 352c 3735 2c38  ,,1595,2125,75,8
-00005d10: 332c 3330 332e 3635 2c33 3138 2e38 3334  3,303.65,318.834
-00005d20: 3935 3135 2c5b 332e 3534 2d20 322e 3036  9515,[3.54- 2.06
-00005d30: 2d20 312e 342d 2031 2e30 2d20 302e 3731  - 1.4- 1.0- 0.71
-00005d40: 2d20 302e 3538 5d2c 3135 3437 2e30 3735  - 0.58],1547.075
-00005d50: 2c31 3632 322e 3037 352c 3136 3437 2e30  ,1622.075,1647.0
-00005d60: 3735 2c31 3539 302c 322e 3539 3534 352c  75,1590,2.59545,
-00005d70: 450d 0a34 3635 3437 2c46 2c36 3633 3539  E..46547,F,66359
-00005d80: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00005d90: 2c2c 7965 732c 7965 732c 7965 732c 6e6f  ,,yes,yes,yes,no
-00005da0: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
-00005db0: 7472 6f6c 2c33 3830 2c38 3330 2c72 6561  trol,380,830,rea
-00005dc0: 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3438  r,,,,,,,,,,,1.48
-00005dd0: 352c 352e 3232 362c 332e 3136 352c 312e  5,5.226,3.165,1.
-00005de0: 3837 312c 2c35 3531 332c 7265 6775 6c61  871,,5513,regula
-00005df0: 722c 3132 2c6f 6863 2c6d 756c 7469 706f  r,12,ohc,multipo
-00005e00: 696e 7420 696e 6a65 6374 696f 6e2c 3930  int injection,90
-00005e10: 2c35 3030 302c 3338 302c 3138 3030 2c38  ,5000,380,1800,8
-00005e20: 3330 2c79 6573 2c33 2c73 6564 616e 2c34  30,yes,3,sedan,4
-00005e30: 2c32 3031 332c 3233 3934 3530 2c35 2c32  ,2013,239450,5,2
-00005e40: 3031 312c 6175 746f 6d61 7469 632c 342e  011,automatic,4.
-00005e50: 362c 3134 2e31 2c33 3239 2c47 2c39 2e37  6,14.1,329,G,9.7
-00005e60: 2c32 3530 2c32 312e 352c 322e 3635 2c32  ,250,21.5,2.65,2
-00005e70: 3035 302c 3231 3130 2c32 3639 302c 3130  050,2110,2690,10
-00005e80: 302c 3837 2c33 3138 2e31 3035 2c33 3333  0,87,318.105,333
-00005e90: 2e33 3439 3531 3436 2c5b 332e 362d 2032  .3495146,[3.6- 2
-00005ea0: 2e31 392d 2031 2e34 2d20 312e 302d 2030  .19- 1.4- 1.0- 0
-00005eb0: 2e38 335d 2c32 3034 392e 3235 2c32 3132  .83],2049.25,212
-00005ec0: 342e 3235 2c32 3134 392e 3235 2c32 3135  4.25,2149.25,215
-00005ed0: 302c 322e 3737 3834 3335 2c46 0d0a 3434  0,2.778435,F..44
-00005ee0: 3739 392c 462c 3633 3736 322c 7965 732c  799,F,63762,yes,
-00005ef0: 7965 732c 7965 732c 7965 732c 2c6e 6f2c  yes,yes,yes,,no,
-00005f00: 3131 3435 2c79 6573 2c79 6573 2c2c 6675  1145,yes,yes,,fu
-00005f10: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
-00005f20: 2c31 3530 2c35 3030 2c72 6561 722c 2c2c  ,150,500,rear,,,
-00005f30: 2c2c 2c2c 2c2c 2c2c 312e 3438 352c 352e  ,,,,,,,,1.485,5.
-00005f40: 3039 362c 332e 3033 352c 312e 3837 312c  096,3.035,1.871,
-00005f50: 2c32 3134 332c 7061 7274 6963 6c65 2066  ,2143,particle f
-00005f60: 696c 7465 722c 342c 646f 6863 2c63 6f6d  ilter,4,dohc,com
-00005f70: 6d6f 6e20 7261 696c 2c38 332c 3432 3030  mon rail,83,4200
-00005f80: 2c31 3530 2c31 3630 302c 3530 302c 7965  ,150,1600,500,ye
-00005f90: 732c 342c 7365 6461 6e2c 342c 3230 3133  s,4,sedan,4,2013
-00005fa0: 2c38 3739 3530 2c35 2c32 3031 312c 6175  ,87950,5,2011,au
-00005fb0: 746f 6d61 7469 632c 382e 322c 352e 372c  tomatic,8.2,5.7,
-00005fc0: 3134 392c 432c 352c 3234 302c 372c 322e  149,C,5,240,7,2.
-00005fd0: 3832 2c31 3930 302c 3138 3730 2c32 3536  82,1900,1870,256
-00005fe0: 352c 3130 302c 3939 2c33 3136 2e37 3135  5,100,99,316.715
-00005ff0: 2c33 3335 2e30 3937 3038 3734 2c5b 342e  ,335.0970874,[4.
-00006000: 3338 2d20 322e 3836 2d20 312e 3932 2d20  38- 2.86- 1.92- 
-00006010: 312e 3337 2d20 312e 302d 2030 2e38 322d  1.37- 1.0- 0.82-
-00006020: 2030 2e37 335d 2c31 3831 332e 3937 352c   0.73],1813.975,
-00006030: 3138 3838 2e39 3735 2c31 3931 332e 3937  1888.975,1913.97
-00006040: 352c 3139 3330 2c32 2e37 3738 3433 352c  5,1930,2.778435,
-00006050: 460d 0a34 3130 3435 2c46 2c35 3833 3632  F..41045,F,58362
-00006060: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00006070: 2c2c 7965 732c 7965 732c 7965 732c 7965  ,,yes,yes,yes,ye
-00006080: 732c 2c66 7565 6c20 656e 6769 6e65 2c70  s,,fuel engine,p
-00006090: 6574 726f 6c2c 3336 382c 3632 352c 6672  etrol,368,625,fr
-000060a0: 6f6e 742b 7265 6172 2c2c 2c2c 2c2c 2c2c  ont+rear,,,,,,,,
-000060b0: 2c2c 2c31 2e34 3731 2c35 2e32 3635 2c33  ,,,1.471,5.265,3
-000060c0: 2e31 3232 2c31 2e39 3439 2c2c 3632 3939  .122,1.949,,6299
-000060d0: 2c72 6567 756c 6172 2c31 322c 646f 6863  ,regular,12,dohc
-000060e0: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
-000060f0: 6e2c 3832 2c36 3230 302c 3336 382c 3437  n,82,6200,368,47
-00006100: 3530 2c36 3235 2c6e 6f2c 342c 7365 6461  50,625,no,4,seda
-00006110: 6e2c 342c 6176 6169 6c61 626c 652c 3232  n,4,available,22
-00006120: 3536 3530 2c35 2c32 3031 342c 6175 746f  5650,5,2014,auto
-00006130: 6d61 7469 632c 342e 362c 3131 2e33 2c32  matic,4.6,11.3,2
-00006140: 3634 2c47 2c38 2e37 2c32 3530 2c31 352e  64,G,8.7,250,15.
-00006150: 372c 332e 3038 2c31 3835 302c 3230 3530  7,3.08,1850,2050
-00006160: 2c32 3637 352c 3130 302c 3930 2e34 2c33  ,2675,100,90.4,3
-00006170: 3330 2e38 3035 2c33 3435 2e36 3739 3631  30.805,345.67961
-00006180: 3137 2c5b 342e 3731 2d20 332e 3134 2d20  17,[4.71- 3.14- 
-00006190: 322e 3131 2d20 312e 3637 2d20 312e 3239  2.11- 1.67- 1.29
-000061a0: 2d20 312e 302d 2030 2e38 342d 2030 2e36  - 1.0- 0.84- 0.6
-000061b0: 375d 2c31 3939 342e 3635 2c32 3036 392e  7],1994.65,2069.
-000061c0: 3635 2c32 3039 342e 3635 2c32 3034 302c  65,2094.65,2040,
-000061d0: 322e 3836 3639 3739 2c46 0d0a 3339 3832  2.866979,F..3982
-000061e0: 302c 462c 3536 3634 312c 7965 732c 7965  0,F,56641,yes,ye
-000061f0: 732c 7965 732c 7965 732c 2c31 3437 312c  s,yes,yes,,1471,
-00006200: 7965 732c 7965 732c 7965 732c 2c66 7565  yes,yes,yes,,fue
-00006210: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
-00006220: 3139 302c 3538 302c 6672 6f6e 742b 7265  190,580,front+re
-00006230: 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  ar,,,,,,,,,,,1.4
-00006240: 362c 352e 3236 352c 332e 3132 322c 312e  6,5.265,3.122,1.
-00006250: 3934 392c 2c32 3936 372c 7061 7274 6963  949,,2967,partic
-00006260: 6c65 2066 696c 7465 722c 362c 646f 6863  le filter,6,dohc
-00006270: 2c63 6f6d 6d6f 6e20 7261 696c 2c38 322c  ,common rail,82,
-00006280: 3430 3030 2c31 3930 2c31 3735 302c 3538  4000,190,1750,58
-00006290: 302c 7965 732c 342c 7365 6461 6e2c 342c  0,yes,4,sedan,4,
-000062a0: 6176 6169 6c61 626c 652c 3130 3131 3330  available,101130
-000062b0: 2c35 2c32 3031 332c 6175 746f 6d61 7469  ,5,2013,automati
-000062c0: 632c 362e 312c 362c 3135 382c 422c 352e  c,6.1,6,158,B,5.
-000062d0: 322c 3235 302c 372e 352c 322e 3338 2c31  2,250,7.5,2.38,1
-000062e0: 3430 302c 3139 3130 2c32 3538 352c 3130  400,1910,2585,10
-000062f0: 302c 3931 2e34 2c33 3239 2e34 3135 2c33  0,91.4,329.415,3
-00006300: 3437 2e34 3237 3138 3435 2c5b 342e 3731  47.4271845,[4.71
-00006310: 2d20 332e 3134 2d20 322e 3131 2d20 312e  - 3.14- 2.11- 1.
-00006320: 3637 2d20 312e 3239 2d20 312e 302d 2030  67- 1.29- 1.0- 0
-00006330: 2e38 342d 2030 2e36 375d 2c31 3835 342e  .84- 0.67],1854.
-00006340: 3635 2c31 3932 392e 3635 2c31 3935 342e  65,1929.65,1954.
-00006350: 3635 2c31 3933 302c 322e 3834 3535 342c  65,1930,2.84554,
-00006360: 460d 0a33 3431 3833 2c46 2c34 3836 3330  F..34183,F,48630
-00006370: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00006380: 2c2c 6e6f 2c79 6573 2c79 6573 2c79 6573  ,,no,yes,yes,yes
-00006390: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
-000063a0: 7472 6f6c 2c32 3238 2c34 3030 2c66 726f  trol,228,400,fro
-000063b0: 6e74 2b72 6561 722c 2c2c 2c2c 2c2c 2c2c  nt+rear,,,,,,,,,
-000063c0: 2c2c 312e 3431 382c 352e 3031 352c 322e  ,,1.418,5.015,2.
-000063d0: 3932 2c31 2e39 3331 2c2c 3336 3035 2c72  92,1.931,,3605,r
-000063e0: 6567 756c 6172 2c36 2c64 6f68 632c 6469  egular,6,dohc,di
-000063f0: 7265 6374 2069 6e6a 6563 7469 6f6e 2c31  rect injection,1
-00006400: 3030 2c36 3230 302c 3232 382c 3337 3530  00,6200,228,3750
-00006410: 2c34 3030 2c6e 6f2c 342c 6861 7463 6862  ,400,no,4,hatchb
-00006420: 6163 6b2c 352c 6176 6169 6c61 626c 652c  ack,5,available,
-00006430: 3131 3335 3030 2c34 2c32 3031 332c 6175  113500,4,2013,au
-00006440: 746f 6d61 7469 632c 362e 312c 382e 372c  tomatic,6.1,8.7,
-00006450: 3230 332c 442c 372e 312c 3235 372c 3131  203,D,7.1,257,11
-00006460: 2e34 2c33 2e39 2c32 3130 302c 3138 3230  .4,3.9,2100,1820
-00006470: 2c32 3432 302c 3735 2c38 332c 3332 342e  ,2420,75,83,324.
-00006480: 3135 2c33 3430 2e38 3733 3738 3634 2c5b  15,340.8737864,[
-00006490: 352e 3937 2d20 332e 3331 2d20 322e 3031  5.97- 3.31- 2.01
-000064a0: 2d20 312e 3337 2d20 312e 302d 2030 2e38  - 1.37- 1.0- 0.8
-000064b0: 312d 2030 2e35 395d 2c31 3735 322e 352c  1- 0.59],1752.5,
-000064c0: 3138 3237 2e35 2c31 3835 322e 352c 3138  1827.5,1852.5,18
-000064d0: 3130 2c32 2e37 3338 3135 382c 460d 0a33  10,2.738158,F..3
-000064e0: 3431 3836 2c46 2c34 3836 3334 2c79 6573  4186,F,48634,yes
-000064f0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-00006500: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-00006510: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
-00006520: 2c32 3231 2c36 3530 2c72 6561 722c 2c2c  ,221,650,rear,,,
-00006530: 2c2c 2c2c 2c2c 2c2c 312e 3431 382c 352e  ,,,,,,,,1.418,5.
-00006540: 3031 352c 322e 3932 2c31 2e39 3331 2c2c  015,2.92,1.931,,
-00006550: 3239 3637 2c70 6172 7469 636c 6520 6669  2967,particle fi
-00006560: 6c74 6572 2c36 2c64 6f68 632c 636f 6d6d  lter,6,dohc,comm
-00006570: 6f6e 2072 6169 6c2c 3830 2c34 3030 302c  on rail,80,4000,
-00006580: 3232 312c 3137 3530 2c36 3530 2c79 6573  221,1750,650,yes
-00006590: 2c34 2c68 6174 6368 6261 636b 2c35 2c61  ,4,hatchback,5,a
-000065a0: 7661 696c 6162 6c65 2c31 3036 3430 302c  vailable,106400,
-000065b0: 342c 3230 3134 2c61 7574 6f6d 6174 6963  4,2014,automatic
-000065c0: 2c36 2c36 2e34 2c31 3639 2c44 2c35 2e36  ,6,6.4,169,D,5.6
-000065d0: 2c32 3539 2c37 2e37 2c32 2e36 392c 3137  ,259,7.7,2.69,17
-000065e0: 3030 2c31 3930 302c 3235 3030 2c37 352c  00,1900,2500,75,
-000065f0: 3931 2e34 2c33 3234 2e31 352c 3334 302e  91.4,324.15,340.
-00006600: 3837 3337 3836 342c 5b34 2e39 322d 2032  8737864,[4.92- 2
-00006610: 2e38 312d 2031 2e38 342d 2031 2e34 332d  .81- 1.84- 1.43-
-00006620: 2031 2e32 312d 2031 2e30 2d20 302e 3833   1.21- 1.0- 0.83
-00006630: 2d20 302e 3639 5d2c 3138 3436 2c31 3932  - 0.69],1846,192
-00006640: 312c 3139 3436 2c31 3933 302c 322e 3733  1,1946,1930,2.73
-00006650: 3831 3538 2c46 0d0a 3230 3631 322c 462c  8158,F..20612,F,
-00006660: 3238 3032 312c 7965 732c 7965 732c 7965  28021,yes,yes,ye
-00006670: 732c 7965 732c 2c31 3939 302c 3133 3235  s,yes,,1990,1325
-00006680: 2c79 6573 2c6e 6f2c 2c66 7565 6c20 656e  ,yes,no,,fuel en
-00006690: 6769 6e65 2c70 6574 726f 6c2c 3234 362c  gine,petrol,246,
-000066a0: 3433 302c 6672 6f6e 742b 7265 6172 2c2c  430,front+rear,,
-000066b0: 2c2c 2c2c 2c2c 2c2c 2c31 2e34 352c 352e  ,,,,,,,,,1.45,5.
-000066c0: 3035 392c 322e 3838 312c 312e 3930 332c  059,2.881,1.903,
-000066d0: 2c34 3137 322c 7265 6775 6c61 722c 382c  ,4172,regular,8,
-000066e0: 646f 6863 2c6d 756c 7469 706f 696e 7420  dohc,multipoint 
-000066f0: 696e 6a65 6374 696f 6e2c 3930 2c36 3530  injection,90,650
-00006700: 302c 3234 362c 3335 3030 2c34 3330 2c6e  0,246,3500,430,n
-00006710: 6f2c 342c 7365 6461 6e2c 342c 6176 6169  o,4,sedan,4,avai
-00006720: 6c61 626c 652c 3134 3835 3930 2c35 2c32  lable,148590,5,2
-00006730: 3031 302c 6175 746f 6d61 7469 632c 362e  010,automatic,6.
-00006740: 392c 3132 2e35 2c32 3930 2c47 2c39 2e32  9,12.5,290,G,9.2
-00006750: 2c32 3530 2c31 382e 322c 332e 3331 2c32  ,250,18.2,3.31,2
-00006760: 3130 302c 3230 3832 2c32 3730 302c 3130  100,2082,2700,10
-00006770: 302c 3933 2c33 3136 2e37 3135 2c33 3335  0,93,316.715,335
-00006780: 2e30 3937 3038 3734 2c5b 342e 3137 2d20  .0970874,[4.17- 
-00006790: 322e 3334 2d20 312e 3532 2d20 312e 3134  2.34- 1.52- 1.14
-000067a0: 2d20 302e 3837 2d20 302e 3639 5d2c 3230  - 0.87- 0.69],20
-000067b0: 3231 2e32 352c 3230 3936 2e32 352c 3231  21.25,2096.25,21
-000067c0: 3231 2e32 352c 3230 3430 2c32 2e37 3539  21.25,2040,2.759
-000067d0: 3335 2c46 0d0a 3230 3630 352c 462c 3238  35,F..20605,F,28
-000067e0: 3031 342c 7965 732c 7965 732c 7965 732c  014,yes,yes,yes,
-000067f0: 7965 732c 2c31 3939 302c 7965 732c 7965  yes,,1990,yes,ye
-00006800: 732c 6e6f 2c2c 6675 656c 2065 6e67 696e  s,no,,fuel engin
-00006810: 652c 6469 6573 656c 2c31 3830 2c35 3030  e,diesel,180,500
-00006820: 2c66 726f 6e74 2b72 6561 722c 2c2c 2c2c  ,front+rear,,,,,
-00006830: 2c2c 2c2c 2c2c 312e 3435 2c35 2e30 3539  ,,,,,,1.45,5.059
-00006840: 2c32 2e38 3831 2c31 2e39 3033 2c2c 3239  ,2.881,1.903,,29
-00006850: 3637 2c70 6172 7469 636c 6520 6669 6c74  67,particle filt
-00006860: 6572 2c36 2c64 6f68 632c 636f 6d6d 6f6e  er,6,dohc,common
-00006870: 2072 6169 6c2c 3930 2c34 3030 302c 3138   rail,90,4000,18
-00006880: 302c 3135 3030 2c35 3030 2c79 6573 2c34  0,1500,500,yes,4
-00006890: 2c73 6564 616e 2c34 2c61 7661 696c 6162  ,sedan,4,availab
-000068a0: 6c65 2c31 3038 3839 302c 352c 3230 3133  le,108890,5,2013
-000068b0: 2c61 7574 6f6d 6174 6963 2c38 2e33 2c38  ,automatic,8.3,8
-000068c0: 2e35 2c32 3234 2c47 2c36 2e37 2c32 3338  .5,224,G,6.7,238
-000068d0: 2c31 312e 362c 332e 3333 2c32 3130 302c  ,11.6,3.33,2100,
-000068e0: 3231 3333 2c32 3736 302c 3130 302c 3931  2133,2760,100,91
-000068f0: 2e34 2c33 3133 2e31 382c 3333 342e 3137  .4,313.18,334.17
-00006900: 3437 3537 332c 5b34 2e31 372d 2032 2e33  47573,[4.17- 2.3
-00006910: 342d 2031 2e35 322d 2031 2e31 342d 2030  4- 1.52- 1.14- 0
-00006920: 2e38 372d 2030 2e36 395d 2c32 3037 322e  .87- 0.69],2072.
-00006930: 3235 2c32 3134 372e 3235 2c32 3137 322e  25,2147.25,2172.
-00006940: 3235 2c32 3135 302c 322e 3735 3933 352c  25,2150,2.75935,
-00006950: 460d 0a31 3332 342c 462c 3135 3136 2c79  F..1324,F,1516,y
-00006960: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
-00006970: 6e6f 2c79 6573 2c79 6573 2c6e 6f2c 2c66  no,yes,yes,no,,f
-00006980: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
-00006990: 6c2c 3232 342c 3432 302c 7265 6172 2c2c  l,224,420,rear,,
-000069a0: 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3535 2c35  ,,,,,,,,,1.455,5
-000069b0: 2e32 3135 2c33 2e31 3539 2c31 2e38 362c  .215,3.159,1.86,
-000069c0: 2c34 3139 362c 7265 6775 6c61 722c 382c  ,4196,regular,8,
-000069d0: 646f 6863 2c6d 756c 7469 706f 696e 7420  dohc,multipoint 
-000069e0: 696e 6a65 6374 696f 6e2c 3835 2c36 3030  injection,85,600
-000069f0: 302c 3232 342c 3431 3030 2c34 3230 2c6e  0,224,4100,420,n
-00006a00: 6f2c 342c 7365 6461 6e2c 342c 3230 3039  o,4,sedan,4,2009
-00006a10: 2c31 3231 3039 302c 352c 3230 3039 2c61  ,121090,5,2009,a
-00006a20: 7574 6f6d 6174 6963 2c36 2e36 2c31 312e  utomatic,6.6,11.
-00006a30: 342c 3236 392c 472c 382e 342c 3235 302c  4,269,G,8.4,250,
-00006a40: 3136 2e37 2c32 2e38 372c 3138 3530 2c31  16.7,2.87,1850,1
-00006a50: 3631 352c 3232 3436 2c37 352c 3930 2e33  615,2246,75,90.3
-00006a60: 2c33 3230 2e38 362c 3333 332e 3330 3039  ,320.86,333.3009
-00006a70: 3730 392c 5b34 2e31 372d 2032 2e33 342d  709,[4.17- 2.34-
-00006a80: 2031 2e35 322d 2031 2e31 342d 2030 2e38   1.52- 1.14- 0.8
-00006a90: 372d 2030 2e36 395d 2c31 3535 372e 3632  7- 0.69],1557.62
-00006aa0: 352c 3136 3332 2e36 3235 2c31 3635 372e  5,1632.625,1657.
-00006ab0: 3632 352c 3135 3930 2c32 2e37 3036 332c  625,1590,2.7063,
-00006ac0: 460d 0a39 3838 322c 462c 3132 3337 352c  F..9882,F,12375,
-00006ad0: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
-00006ae0: 2c79 6573 2c79 6573 2c79 6573 2c6e 6f2c  ,yes,yes,yes,no,
-00006af0: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
-00006b00: 726f 6c2c 3330 312c 3535 302c 7265 6172  rol,301,550,rear
-00006b10: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3831  ,,,,,,,,,,,1.481
-00006b20: 2c35 2e32 3632 2c33 2e31 3731 2c31 2e39  ,5.262,3.171,1.9
-00006b30: 3438 2c2c 3239 3739 2c72 6567 756c 6172  48,,2979,regular
-00006b40: 2c36 2c64 6f68 632c 6469 7265 6374 2069  ,6,dohc,direct i
-00006b50: 6e6a 6563 7469 6f6e 2c38 302c 3535 3030  njection,80,5500
-00006b60: 2c33 3031 2c31 3735 302c 3535 302c 7965  ,301,1750,550,ye
-00006b70: 732c 342c 7365 6461 6e2c 342c 6176 6169  s,4,sedan,4,avai
-00006b80: 6c61 626c 652c 3133 3938 3231 2c35 2c32  lable,139821,5,2
-00006b90: 3031 342c 6175 746f 6d61 7469 632c 352e  014,automatic,5.
-00006ba0: 312c 3130 2e35 2c32 3434 2c46 2c37 2e37  1,10.5,244,F,7.7
-00006bb0: 2c32 3835 2c31 352e 332c 332e 3733 2c2c  ,285,15.3,3.73,,
-00006bc0: 3139 3230 2c32 3534 302c 2c38 342e 352c  1920,2540,,84.5,
-00006bd0: 3332 372e 3239 352c 3334 312e 3331 3036  327.295,341.3106
-00006be0: 3739 362c 5b33 2e32 392d 2032 2e31 362d  796,[3.29- 2.16-
-00006bf0: 2031 2e36 312d 2031 2e32 372d 2031 2e30   1.61- 1.27- 1.0
-00006c00: 332d 2030 2e38 355d 2c31 3836 362c 3139  3- 0.85],1866,19
-00006c10: 3431 2c31 3936 362c 3139 3330 2c32 2e38  41,1966,1930,2.8
-00006c20: 3834 3938 382c 460d 0a34 3935 372c 462c  84988,F..4957,F,
-00006c30: 3631 3132 2c79 6573 2c79 6573 2c79 6573  6112,yes,yes,yes
-00006c40: 2c79 6573 2c2c 6e6f 2c79 6573 2c79 6573  ,yes,,no,yes,yes
-00006c50: 2c6e 6f2c 2c66 7565 6c20 656e 6769 6e65  ,no,,fuel engine
-00006c60: 2c70 6574 726f 6c2c 3337 332c 3939 392c  ,petrol,373,999,
-00006c70: 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  rear,,,,,,,,,,,1
-00006c80: 2e35 3135 2c35 2e34 2c33 2e31 3136 2c31  .515,5.4,3.116,1
-00006c90: 2e39 2c2c 3637 3631 2c72 6567 756c 6172  .9,,6761,regular
-00006ca0: 2c38 2c6f 6876 2c6d 756c 7469 706f 696e  ,8,ohv,multipoin
-00006cb0: 7420 696e 6a65 6374 696f 6e2c 3936 2c34  t injection,96,4
-00006cc0: 3230 302c 3337 332c 3332 3030 2c39 3939  200,373,3200,999
-00006cd0: 2c79 6573 2c32 2c73 6564 616e 2c34 2c32  ,yes,2,sedan,4,2
-00006ce0: 3031 302c 2c35 2c32 3030 372c 6175 746f  010,,5,2007,auto
-00006cf0: 6d61 7469 632c 352e 352c 3139 2e35 2c34  matic,5.5,19.5,4
-00006d00: 3635 2c47 2c31 342e 312c 3238 382c 3238  65,G,14.1,288,28
-00006d10: 2e38 2c32 2e36 392c 2c32 3538 352c 3330  .8,2.69,,2585,30
-00006d20: 3635 2c2c 3939 2e31 2c33 3330 2e38 3035  65,,99.1,330.805
-00006d30: 2c33 3435 2e36 3739 3631 3137 2c5b 322e  ,345.6796117,[2.
-00006d40: 3438 2d20 312e 3438 2d20 312e 302d 2030  48- 1.48- 1.0- 0
-00006d50: 2e37 355d 2c32 3532 302e 322c 3235 3935  .75],2520.2,2595
-00006d60: 2e32 2c32 3632 302e 322c 3232 3730 2c32  .2,2620.2,2270,2
-00006d70: 2e38 3738 352c 460d 0a35 3539 352c 532c  .8785,F..5595,S,
-00006d80: 3638 3639 2c79 6573 2c79 6573 2c79 6573  6869,yes,yes,yes
-00006d90: 2c79 6573 2c2c 3936 362c 7965 732c 7965  ,yes,,966,yes,ye
-00006da0: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00006db0: 6e65 2c70 6574 726f 6c2c 3233 352c 3435  ne,petrol,235,45
-00006dc0: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00006dd0: 2c2c 2c2c 2c2c 2c31 2e33 3635 2c34 2e38  ,,,,,,,1.365,4.8
-00006de0: 3934 2c32 2e38 3535 2c31 2e38 3934 2c2c  94,2.855,1.894,,
-00006df0: 3239 3739 2c72 6567 756c 6172 2c36 2c64  2979,regular,6,d
-00006e00: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
-00006e10: 7469 6f6e 2c37 302c 3538 3030 2c32 3335  tion,70,5800,235
-00006e20: 2c31 3330 302c 3435 302c 7965 732c 342c  ,1300,450,yes,4,
-00006e30: 6361 6272 696f 6c65 742c 322c 6176 6169  cabriolet,2,avai
-00006e40: 6c61 626c 652c 3132 3038 3935 2c34 2c32  lable,120895,4,2
-00006e50: 3031 352c 6175 746f 6d61 7469 632c 352e  015,automatic,5.
-00006e60: 342c 382e 322c 3139 312c 442c 362e 332c  4,8.2,191,D,6.3,
-00006e70: 3235 302c 3131 2e34 2c33 2e32 332c 3230  250,11.4,3.23,20
-00006e80: 3530 2c31 3836 352c 3233 3930 2c30 2c38  50,1865,2390,0,8
-00006e90: 392e 362c 3331 342e 3539 352c 3332 382e  9.6,314.595,328.
-00006ea0: 3938 3035 3832 352c 5b34 2e37 312d 2033  9805825,[4.71- 3
-00006eb0: 2e31 342d 2032 2e31 312d 2031 2e36 372d  .14- 2.11- 1.67-
-00006ec0: 2031 2e32 392d 2031 2e30 2d20 302e 3834   1.29- 1.0- 0.84
-00006ed0: 2d20 302e 3637 5d2c 3138 3137 2e37 352c  - 0.67],1817.75,
-00006ee0: 3138 3932 2e37 352c 3139 3137 2e37 352c  1892.75,1917.75,
-00006ef0: 3139 3330 2c32 2e35 3835 3331 2c53 0d0a  1930,2.58531,S..
-00006f00: 3138 3833 312c 532c 3235 3434 352c 7965  18831,S,25445,ye
-00006f10: 732c 7965 732c 7965 732c 6e6f 2c2c 6e6f  s,yes,yes,no,,no
-00006f20: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-00006f30: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
-00006f40: 2c31 3530 2c33 3130 2c72 6561 722c 2c2c  ,150,310,rear,,,
-00006f50: 2c2c 2c2c 2c2c 2c2c 312e 3330 312c 342e  ,,,,,,,,1.301,4.
-00006f60: 3133 342c 322e 3433 2c31 2e38 312c 2c31  134,2.43,1.81,,1
-00006f70: 3739 362c 7265 6775 6c61 722c 342c 646f  796,regular,4,do
-00006f80: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-00006f90: 696f 6e2c 3630 2c35 3530 302c 3135 302c  ion,60,5500,150,
-00006fa0: 3230 3030 2c33 3130 2c79 6573 2c34 2c63  2000,310,yes,4,c
-00006fb0: 6162 7269 6f6c 6574 2c32 2c61 7661 696c  abriolet,2,avail
-00006fc0: 6162 6c65 2c35 3232 3530 2c32 2c32 3031  able,52250,2,201
-00006fd0: 322c 6d61 6e75 616c 2c36 2e35 2c36 2e39  2,manual,6.5,6.9
-00006fe0: 2c31 3630 2c45 2c35 2e33 2c32 3434 2c39  ,160,E,5.3,244,9
-00006ff0: 2e35 2c33 2e32 372c 3237 3530 2c31 3337  .5,3.27,2750,137
-00007000: 352c 3137 3930 2c35 302c 3835 2c32 3934  5,1790,50,85,294
-00007010: 2e38 3735 2c33 3037 2e39 3132 3632 3134  .875,307.9126214
-00007020: 2c5b 342e 3436 2d20 322e 3631 2d20 312e  ,[4.46- 2.61- 1.
-00007030: 3732 2d20 312e 3235 2d20 312e 302d 2030  72- 1.25- 1.0- 0
-00007040: 2e38 345d 2c31 3333 342e 352c 3134 3039  .84],1334.5,1409
-00007050: 2e35 2c31 3433 342e 352c 3133 3630 2c32  .5,1434.5,1360,2
-00007060: 2e33 3534 3831 2c53 0d0a 3138 3833 332c  .35481,S..18833,
-00007070: 532c 3235 3434 372c 7965 732c 7965 732c  S,25447,yes,yes,
-00007080: 7965 732c 6e6f 2c2c 6e6f 2c79 6573 2c79  yes,no,,no,yes,y
-00007090: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
-000070a0: 696e 652c 6469 6573 656c 2c31 3530 2c35  ine,diesel,150,5
-000070b0: 3030 2c72 6561 722c 2c2c 2c2c 2c2c 2c2c  00,rear,,,,,,,,,
-000070c0: 2c2c 312e 3330 312c 342e 3133 342c 322e  ,,1.301,4.134,2.
-000070d0: 3433 2c31 2e38 312c 2c32 3134 332c 7061  43,1.81,,2143,pa
-000070e0: 7274 6963 6c65 2066 696c 7465 722c 342c  rticle filter,4,
-000070f0: 646f 6863 2c63 6f6d 6d6f 6e20 7261 696c  dohc,common rail
-00007100: 2c36 302c 3535 3030 2c31 3530 2c31 3630  ,60,5500,150,160
-00007110: 302c 3530 302c 7965 732c 342c 6361 6272  0,500,yes,4,cabr
-00007120: 696f 6c65 742c 322c 6176 6169 6c61 626c  iolet,2,availabl
-00007130: 652c 3530 3835 302c 322c 3230 3132 2c6d  e,50850,2,2012,m
-00007140: 616e 7561 6c2c 362e 352c 342e 382c 3132  anual,6.5,4.8,12
-00007150: 342c 452c 342c 3234 342c 362e 322c 322e  4,E,4,244,6.2,2.
-00007160: 3437 2c32 3030 302c 3134 3730 2c31 3838  47,2000,1470,188
-00007170: 352c 3530 2c39 392c 3239 312e 3134 352c  5,50,99,291.145,
-00007180: 3330 362e 3734 3735 3732 382c 5b35 2e31  306.7475728,[5.1
-00007190: 2d20 322e 3738 2d20 312e 3735 2d20 312e  - 2.78- 1.75- 1.
-000071a0: 3235 2d20 312e 302d 2030 2e38 315d 2c31  25- 1.0- 0.81],1
-000071b0: 3432 392e 352c 3135 3034 2e35 2c31 3532  429.5,1504.5,152
-000071c0: 392e 352c 3134 3730 2c32 2e33 3534 3831  9.5,1470,2.35481
-000071d0: 2c53 0d0a 3935 3735 2c53 2c31 3138 3230  ,S..9575,S,11820
-000071e0: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-000071f0: 2c2c 6e6f 2c79 6573 2c79 6573 2c79 6573  ,,no,yes,yes,yes
-00007200: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
-00007210: 7472 6f6c 2c31 3335 2c32 3730 2c72 6561  trol,135,270,rea
-00007220: 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3239  r,,,,,,,,,,,1.29
-00007230: 312c 342e 3233 392c 322e 3439 362c 312e  1,4.239,2.496,1.
-00007240: 3739 2c2c 3139 3937 2c72 6567 756c 6172  79,,1997,regular
-00007250: 2c34 2c64 6f68 632c 6469 7265 6374 2069  ,4,dohc,direct i
-00007260: 6e6a 6563 7469 6f6e 2c35 352c 3530 3030  njection,55,5000
-00007270: 2c31 3335 2c31 3235 302c 3237 302c 7965  ,135,1250,270,ye
-00007280: 732c 342c 6361 6272 696f 6c65 742c 322c  s,4,cabriolet,2,
-00007290: 6176 6169 6c61 626c 652c 3531 3339 352c  available,51395,
-000072a0: 322c 3230 3133 2c6d 616e 7561 6c2c 362e  2,2013,manual,6.
-000072b0: 392c 362e 382c 3135 392c 452c 352e 362c  9,6.8,159,E,5.6,
-000072c0: 3233 352c 382e 392c 332e 3733 2c32 3535  235,8.9,3.73,255
-000072d0: 302c 3133 3730 2c31 3732 352c 302c 3930  0,1370,1725,0,90
-000072e0: 2e31 2c32 3934 2e38 3735 2c33 3037 2e39  .1,294.875,307.9
-000072f0: 3132 3632 3134 2c5b 332e 3638 2d20 322e  126214,[3.68- 2.
-00007300: 3036 2d20 312e 3331 2d20 312e 302d 2030  06- 1.31- 1.0- 0
-00007310: 2e38 312d 2030 2e36 385d 2c31 3333 322e  .81- 0.68],1332.
-00007320: 3837 352c 3134 3037 2e38 3735 2c31 3433  875,1407.875,143
-00007330: 322e 3837 352c 3133 3630 2c32 2e33 3130  2.875,1360,2.310
-00007340: 3839 2c53 0d0a 3533 3830 2c53 2c36 3635  89,S..5380,S,665
-00007350: 312c 7965 732c 7965 732c 7965 732c 7965  1,yes,yes,yes,ye
-00007360: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
-00007370: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
-00007380: 6965 7365 6c2c 3133 352c 3338 302c 6672  iesel,135,380,fr
-00007390: 6f6e 742c 2c2c 2c2c 2c2c 2c2c 2c2c 312e  ont,,,,,,,,,,,1.
-000073a0: 3335 352c 342e 3137 372c 322e 3530 352c  355,4.177,2.505,
-000073b0: 312e 3833 322c 2c31 3938 342c 7061 7274  1.832,,1984,part
-000073c0: 6963 6c65 2066 696c 7465 722c 342c 646f  icle filter,4,do
-000073d0: 6863 2c63 6f6d 6d6f 6e20 7261 696c 2c35  hc,common rail,5
-000073e0: 302c 3335 3030 2c31 3335 2c31 3735 302c  0,3500,135,1750,
-000073f0: 3338 302c 7965 732c 342c 6361 6272 696f  380,yes,4,cabrio
-00007400: 6c65 742c 322c 6176 6169 6c61 626c 652c  let,2,available,
-00007410: 3534 3331 302c 342c 3230 3135 2c6d 616e  54310,4,2015,man
-00007420: 7561 6c2c 372e 332c 342e 332c 3131 342c  ual,7.3,4.3,114,
-00007430: 442c 332e 392c 3233 372c 352e 312c 322e  D,3.9,237,5.1,2.
-00007440: 3736 2c32 3035 302c 3133 3335 2c31 3638  76,2050,1335,168
-00007450: 302c 3735 2c39 322e 382c 3330 332e 3635  0,75,92.8,303.65
-00007460: 2c33 3138 2e38 3334 3935 3135 2c5b 332e  ,318.8349515,[3.
-00007470: 3737 2d20 322e 3039 2d20 312e 3332 2d20  77- 2.09- 1.32- 
-00007480: 302e 3932 2d20 302e 392d 2030 2e37 365d  0.92- 0.9- 0.76]
-00007490: 2c31 3330 312e 3235 2c31 3337 362e 3235  ,1301.25,1376.25
-000074a0: 2c31 3430 312e 3235 2c31 3336 302c 322e  ,1401.25,1360,2.
-000074b0: 3438 3233 362c 530d 0a39 3933 362c 532c  48236,S..9936,S,
-000074c0: 3132 3432 392c 7965 732c 7965 732c 7965  12429,yes,yes,ye
-000074d0: 732c 6e6f 2c2c 6e6f 2c6e 6f2c 7965 732c  s,no,,no,no,yes,
-000074e0: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
-000074f0: 7065 7472 6f6c 2c39 332c 3136 372c 7265  petrol,93,167,re
-00007500: 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e32  ar,,,,,,,,,,,1.2
-00007510: 3435 2c34 2e30 322c 322e 3333 2c31 2e37  45,4.02,2.33,1.7
-00007520: 322c 2c31 3739 382c 7265 6775 6c61 722c  2,,1798,regular,
-00007530: 342c 646f 6863 2c6d 756c 7469 706f 696e  4,dohc,multipoin
-00007540: 7420 696e 6a65 6374 696f 6e2c 3530 2c36  t injection,50,6
-00007550: 3530 302c 3933 2c34 3530 302c 3136 372c  500,93,4500,167,
-00007560: 6e6f 2c34 2c63 6162 7269 6f6c 6574 2c32  no,4,cabriolet,2
-00007570: 2c61 7661 696c 6162 6c65 2c33 3134 3930  ,available,31490
-00007580: 2c32 2c32 3031 342c 6d61 6e75 616c 2c39  ,2,2014,manual,9
-00007590: 2e39 2c37 2e31 2c31 3637 2c46 2c35 2e36  .9,7.1,167,F,5.6
-000075a0: 2c31 3934 2c39 2e38 2c34 2e31 2c33 3430  ,194,9.8,4.1,340
-000075b0: 302c 3130 3530 2c31 3337 352c 2c38 332e  0,1050,1375,,83.
-000075c0: 312c 3238 372e 3835 352c 3239 392e 3137  1,287.855,299.17
-000075d0: 3437 3537 332c 5b33 2e31 342d 2031 2e38  47573,[3.14- 1.8
-000075e0: 392d 2031 2e33 332d 2031 2e30 2d20 302e  9- 1.33- 1.0- 0.
-000075f0: 3831 5d2c 3130 3136 2e32 352c 3130 3931  81],1016.25,1091
-00007600: 2e32 352c 3131 3136 2e32 352c 3131 3330  .25,1116.25,1130
-00007610: 2c32 2e31 3431 342c 530d 0a37 3939 352c  ,2.1414,S..7995,
-00007620: 532c 3935 3833 2c79 6573 2c79 6573 2c34  S,9583,yes,yes,4
-00007630: 3136 2c6e 6f2c 2c6e 6f2c 3534 312c 7965  16,no,,no,541,ye
-00007640: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00007650: 6e65 2c70 6574 726f 6c2c 3234 332c 3337  ne,petrol,243,37
-00007660: 302c 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c  0,rear,,,,,,,,,,
-00007670: 2c31 2e32 3733 2c34 2e34 3034 2c32 2e34  ,1.273,4.404,2.4
-00007680: 3735 2c31 2e38 3031 2c2c 3334 3336 2c72  75,1.801,,3436,r
-00007690: 6567 756c 6172 2c36 2c64 6f68 632c 6469  egular,6,dohc,di
-000076a0: 7265 6374 2069 6e6a 6563 7469 6f6e 2c36  rect injection,6
-000076b0: 342c 3637 3030 2c32 3433 2c34 3530 302c  4,6700,243,4500,
-000076c0: 3337 302c 6e6f 2c34 2c63 6162 7269 6f6c  370,no,4,cabriol
-000076d0: 6574 2c32 2c61 7661 696c 6162 6c65 2c39  et,2,available,9
-000076e0: 3238 3030 2c32 2c32 3031 342c 6175 746f  2800,2,2014,auto
-000076f0: 6d61 7469 632c 342e 392c 382e 322c 3139  matic,4.9,8.2,19
-00007700: 302c 462c 362e 332c 3237 392c 3131 2e34  0,F,6.3,279,11.4
-00007710: 2c33 2e32 352c 3139 3030 2c31 3335 302c  ,3.25,1900,1350,
-00007720: 3136 3835 2c37 352c 3737 2e35 2c33 3138  1685,75,77.5,318
-00007730: 2e31 3535 2c33 3236 2e34 3536 3331 3037  .155,326.4563107
-00007740: 2c5b 332e 3931 2d20 322e 3239 2d20 312e  ,[3.91- 2.29- 1.
-00007750: 3635 2d20 312e 332d 2031 2e30 382d 2030  65- 1.3- 1.08- 0
-00007760: 2e38 382d 2030 2e36 325d 2c31 3330 362e  .88- 0.62],1306.
-00007770: 382c 3133 3831 2e38 2c31 3430 362e 382c  8,1381.8,1406.8,
-00007780: 3133 3630 2c32 2e32 3932 3637 332c 530d  1360,2.292673,S.
-00007790: 0a36 3333 312c 532c 3737 3236 2c79 6573  .6331,S,7726,yes
-000077a0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-000077b0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
-000077c0: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
-000077d0: 2c34 3132 2c37 3535 2c72 6561 722c 2c2c  ,412,755,rear,,,
-000077e0: 2c2c 2c2c 2c2c 2c2c 312e 3332 322c 342e  ,,,,,,,,1.322,4.
-000077f0: 3537 2c32 2e36 372c 312e 3931 2c2c 3338  57,2.67,1.91,,38
-00007800: 3535 2c72 6567 756c 6172 2c38 2c64 6f68  55,regular,8,doh
-00007810: 632c 6469 7265 6374 2069 6e6a 6563 7469  c,direct injecti
-00007820: 6f6e 2c37 382c 3735 3030 2c34 3132 2c34  on,78,7500,412,4
-00007830: 3735 302c 3735 352c 7965 732c 342c 6361  750,755,yes,4,ca
-00007840: 6272 696f 6c65 742c 322c 6176 6169 6c61  briolet,2,availa
-00007850: 626c 652c 3232 3333 3438 2c34 2c32 3031  ble,223348,4,201
-00007860: 342c 6175 746f 6d61 7469 632c 332e 362c  4,automatic,3.6,
-00007870: 3130 2e35 2c32 3530 2c47 2c2c 3331 362c  10.5,250,G,,316,
-00007880: 2c34 2e34 342c 3330 3030 2c31 3632 352c  ,4.44,3000,1625,
-00007890: 2c2c 3832 2c33 3137 2e37 342c 3332 392e  ,,82,317.74,329.
-000078a0: 3431 3734 3735 372c 5b33 2e34 2d20 322e  4174757,[3.4- 2.
-000078b0: 3139 2d20 312e 3633 2d20 312e 3239 2d20  19- 1.63- 1.29- 
-000078c0: 312e 3033 2d20 302e 3834 2d20 302e 3732  1.03- 0.84- 0.72
-000078d0: 5d2c 3135 3732 2e33 352c 3136 3437 2e33  ],1572.35,1647.3
-000078e0: 352c 3136 3732 2e33 352c 3137 3030 2c32  5,1672.35,1700,2
-000078f0: 2e35 3235 3032 2c53 0d0a 3138 3137 332c  .52502,S..18173,
-00007900: 532c 3234 3438 352c 7965 732c 7965 732c  S,24485,yes,yes,
-00007910: 6e6f 2c79 6573 2c2c 6e6f 2c6e 6f2c 7965  no,yes,,no,no,ye
-00007920: 732c 6e6f 2c2c 6675 656c 2065 6e67 696e  s,no,,fuel engin
-00007930: 652c 7065 7472 6f6c 2c34 3139 2c35 3430  e,petrol,419,540
-00007940: 2c66 726f 6e74 2b72 6561 722c 2c2c 2c2c  ,front+rear,,,,,
-00007950: 2c2c 2c2c 2c2c 312e 3138 342c 342e 3338  ,,,,,,1.184,4.38
-00007960: 362c 322e 3536 2c31 2e39 2c2c 3532 3034  6,2.56,1.9,,5204
-00007970: 2c72 6567 756c 6172 2c31 302c 646f 6863  ,regular,10,dohc
-00007980: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
-00007990: 6e2c 3830 2c38 3030 302c 3431 392c 3635  n,80,8000,419,65
-000079a0: 3030 2c35 3430 2c6e 6f2c 342c 6361 6272  00,540,no,4,cabr
-000079b0: 696f 6c65 742c 322c 3230 3133 2c33 3138  iolet,2,2013,318
-000079c0: 3537 302c 322c 3230 3132 2c6d 616e 7561  570,2,2012,manua
-000079d0: 6c2c 332e 392c 3133 2e36 2c33 3237 2c47  l,3.9,13.6,327,G
-000079e0: 2c39 2e36 2c33 3234 2c32 302e 352c 332e  ,9.6,324,20.5,3.
-000079f0: 3038 2c32 3435 302c 3134 3835 2c31 3830  08,2450,1485,180
-00007a00: 302c 2c39 322e 382c 3330 352e 3435 352c  0,,92.8,305.455,
-00007a10: 3331 342e 3132 3632 3133 362c 5b32 2e35  314.1262136,[2.5
-00007a20: 362d 2031 2e38 352d 2031 2e34 322d 2031  6- 1.85- 1.42- 1
-00007a30: 2e31 342d 2030 2e39 342d 2030 2e38 315d  .14- 0.94- 0.81]
-00007a40: 2c31 3433 312c 3135 3036 2c31 3533 312c  ,1431,1506,1531,
-00007a50: 3134 3730 2c32 2e32 3439 362c 530d 0a33  1470,2.2496,S..3
-00007a60: 3432 3836 2c4d 2c34 3837 3431 2c79 6573  4286,M,48741,yes
-00007a70: 2c79 6573 2c79 6573 2c79 6573 2c2c 7965  ,yes,yes,yes,,ye
-00007a80: 732c 7965 732c 7965 732c 7965 732c 2c66  s,yes,yes,yes,,f
-00007a90: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
-00007aa0: 6c2c 3835 2c31 3930 2c66 726f 6e74 2c2c  l,85,190,front,,
-00007ab0: 2c2c 2c2c 2c2c 2c2c 2c31 2e36 342c 342e  ,,,,,,,,,1.64,4.
-00007ac0: 3336 362c 322e 3730 322c 312e 3834 352c  366,2.702,1.845,
-00007ad0: 2c31 3139 382c 7265 6775 6c61 722c 342c  ,1198,regular,4,
-00007ae0: 646f 6863 2c64 6972 6563 7420 696e 6a65  dohc,direct inje
-00007af0: 6374 696f 6e2c 3630 2c34 3530 302c 3835  ction,60,4500,85
-00007b00: 2c32 3030 302c 3139 302c 7965 732c 342c  ,2000,190,yes,4,
-00007b10: 6d70 762c 352c 3230 3135 2c32 3736 3930  mpv,5,2015,27690
-00007b20: 2c35 2c32 3031 342c 6d61 6e75 616c 2c31  ,5,2014,manual,1
-00007b30: 312e 372c 352e 392c 3133 352c 422c 352e  1.7,5.9,135,B,5.
-00007b40: 322c 3138 352c 372e 322c 342e 3733 2c33  2,185,7.2,4.73,3
-00007b50: 3335 302c 3132 3935 2c31 3935 352c 2c37  350,1295,1955,,7
-00007b60: 332e 312c 3330 332e 3834 352c 3331 392e  3.1,303.845,319.
-00007b70: 3037 3736 3639 392c 5b33 2e37 332d 2032  0776699,[3.73- 2
-00007b80: 2e31 312d 2031 2e34 352d 2031 2e30 392d  .11- 1.45- 1.09-
-00007b90: 2030 2e38 372d 2030 2e37 335d 2c31 3235   0.87- 0.73],125
-00007ba0: 342e 352c 3133 3239 2e35 2c31 3335 342e  4.5,1329.5,1354.
-00007bb0: 352c 3133 3630 2c33 2e30 3235 382c 4d0d  5,1360,3.0258,M.
-00007bc0: 0a33 3432 3739 2c4d 2c34 3837 3334 2c79  .34279,M,48734,y
-00007bd0: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
-00007be0: 6e6f 2c79 6573 2c79 6573 2c79 6573 2c2c  no,yes,yes,yes,,
-00007bf0: 6675 656c 2065 6e67 696e 652c 6469 6573  fuel engine,dies
-00007c00: 656c 2c38 312c 3236 302c 6672 6f6e 742c  el,81,260,front,
-00007c10: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3634 2c34  ,,,,,,,,,,1.64,4
-00007c20: 2e33 3636 2c32 2e37 3032 2c31 2e38 3435  .366,2.702,1.845
-00007c30: 2c2c 3134 3631 2c70 6172 7469 636c 6520  ,,1461,particle 
-00007c40: 6669 6c74 6572 2c34 2c64 6f68 632c 636f  filter,4,dohc,co
-00007c50: 6d6d 6f6e 2072 6169 6c2c 3630 2c34 3030  mmon rail,60,400
-00007c60: 302c 3831 2c31 3735 302c 3236 302c 7965  0,81,1750,260,ye
-00007c70: 732c 322c 6d70 762c 352c 6176 6169 6c61  s,2,mpv,5,availa
-00007c80: 626c 652c 3330 3739 302c 352c 3230 3134  ble,30790,5,2014
-00007c90: 2c6d 616e 7561 6c2c 3132 2e35 2c34 2e31  ,manual,12.5,4.1
-00007ca0: 2c31 3035 2c42 2c33 2e39 2c31 3830 2c34  ,105,B,3.9,180,4
-00007cb0: 2e35 2c34 2e31 332c 3235 3530 2c31 3336  .5,4.13,2550,136
-00007cc0: 302c 3139 3637 2c2c 3830 2e35 2c32 3939  0,1967,,80.5,299
-00007cd0: 2e31 342c 3331 362e 3639 3930 3239 312c  .14,316.6990291,
-00007ce0: 5b33 2e37 332d 2031 2e39 362d 2031 2e33  [3.73- 1.96- 1.3
-00007cf0: 322d 2030 2e39 382d 2030 2e37 362d 2030  2- 0.98- 0.76- 0
-00007d00: 2e36 345d 2c31 3331 392e 352c 3133 3934  .64],1319.5,1394
-00007d10: 2e35 2c31 3431 392e 352c 3133 3630 2c33  .5,1419.5,1360,3
-00007d20: 2e30 3235 382c 4d0d 0a32 3037 3036 2c4d  .0258,M..20706,M
-00007d30: 2c32 3831 3135 2c79 6573 2c79 6573 2c79  ,28115,yes,yes,y
-00007d40: 6573 2c79 6573 2c2c 6e6f 2c35 3835 2c79  es,yes,,no,585,y
-00007d50: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
-00007d60: 696e 652c 6469 6573 656c 2c37 372c 3235  ine,diesel,77,25
-00007d70: 302c 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c  0,front,,,,,,,,,
-00007d80: 2c2c 312e 3637 342c 342e 3339 372c 322e  ,,1.674,4.397,2.
-00007d90: 3637 382c 312e 3739 342c 2c31 3539 382c  678,1.794,,1598,
-00007da0: 7061 7274 6963 6c65 2066 696c 7465 722c  particle filter,
-00007db0: 342c 646f 6863 2c63 6f6d 6d6f 6e20 7261  4,dohc,common ra
-00007dc0: 696c 2c36 302c 3434 3030 2c37 372c 3135  il,60,4400,77,15
-00007dd0: 3030 2c32 3530 2c79 6573 2c34 2c6d 7076  00,250,yes,4,mpv
-00007de0: 2c35 2c32 3031 352c 3335 3339 302c 372c  ,5,2015,35390,7,
-00007df0: 3230 3134 2c6d 616e 7561 6c2c 3132 2e38  2014,manual,12.8
-00007e00: 2c34 2e36 2c31 3231 2c45 2c34 2e31 2c31  ,4.6,121,E,4.1,1
-00007e10: 3836 2c35 2e35 2c33 2e36 352c 3233 3030  86,5.5,3.65,2300
-00007e20: 2c31 3434 342c 3231 3830 2c31 3030 2c38  ,1444,2180,100,8
-00007e30: 302e 352c 3239 312e 3134 352c 3330 362e  0.5,291.145,306.
-00007e40: 3734 3735 3732 382c 5b34 2e31 312d 2032  7475728,[4.11- 2
-00007e50: 2e31 322d 2031 2e33 362d 2030 2e39 372d  .12- 1.36- 0.97-
-00007e60: 2030 2e37 372d 2030 2e36 335d 2c31 3430   0.77- 0.63],140
-00007e70: 332e 352c 3134 3738 2e35 2c31 3530 332e  3.5,1478.5,1503.
-00007e80: 352c 3134 3730 2c33 2e30 3033 3135 362c  5,1470,3.003156,
-00007e90: 4d0d 0a33 3430 3538 2c4d 2c34 3834 3934  M..34058,M,48494
-00007ea0: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
-00007eb0: 2c2c 6e6f 2c79 6573 2c79 6573 2c6e 6f2c  ,,no,yes,yes,no,
-00007ec0: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
-00007ed0: 726f 6c2c 3131 352c 3234 302c 6672 6f6e  rol,115,240,fron
-00007ee0: 742c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3633  t,,,,,,,,,,,1.63
-00007ef0: 392c 342e 3336 352c 322e 3631 332c 312e  9,4.365,2.613,1.
-00007f00: 3833 372c 2c31 3539 382c 7265 6775 6c61  837,,1598,regula
-00007f10: 722c 342c 646f 6863 2c64 6972 6563 7420  r,4,dohc,direct 
-00007f20: 696e 6a65 6374 696f 6e2c 3630 2c36 3030  injection,60,600
-00007f30: 302c 3131 352c 3134 3030 2c32 3430 2c79  0,115,1400,240,y
-00007f40: 6573 2c34 2c6d 7076 2c35 2c61 7661 696c  es,4,mpv,5,avail
-00007f50: 6162 6c65 2c33 3139 3530 2c35 2c32 3031  able,31950,5,201
-00007f60: 342c 6d61 6e75 616c 2c38 2e39 2c36 2e39  4,manual,8.9,6.9
-00007f70: 2c31 3539 2c44 2c35 2e35 2c32 3032 2c39  ,159,D,5.5,202,9
-00007f80: 2e33 2c34 2e31 382c 3237 3530 2c31 3433  .3,4.18,2750,143
-00007f90: 342c 3230 3230 2c37 352c 3835 2e38 2c33  4,2020,75,85.8,3
-00007fa0: 3033 2e36 352c 3331 382e 3833 3439 3531  03.65,318.834951
-00007fb0: 352c 5b33 2e35 342d 2031 2e39 322d 2031  5,[3.54- 1.92- 1
-00007fc0: 2e33 332d 2031 2e30 332d 2030 2e38 322d  .33- 1.03- 0.82-
-00007fd0: 2030 2e36 385d 2c31 3339 332e 352c 3134   0.68],1393.5,14
-00007fe0: 3638 2e35 2c31 3439 332e 352c 3134 3730  68.5,1493.5,1470
-00007ff0: 2c33 2e30 3130 3834 332c 4d0d 0a33 3430  ,3.010843,M..340
-00008000: 3537 2c4d 2c34 3834 3933 2c79 6573 2c79  57,M,48493,yes,y
-00008010: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
-00008020: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
-00008030: 2065 6e67 696e 652c 6469 6573 656c 2c38   engine,diesel,8
-00008040: 352c 3237 302c 6672 6f6e 742c 2c2c 2c2c  5,270,front,,,,,
-00008050: 2c2c 2c2c 2c2c 312e 3633 392c 342e 3336  ,,,,,,1.639,4.36
-00008060: 352c 322e 3631 332c 312e 3833 372c 2c31  5,2.613,1.837,,1
-00008070: 3536 302c 7061 7274 6963 6c65 2066 696c  560,particle fil
-00008080: 7465 722c 342c 646f 6863 2c63 6f6d 6d6f  ter,4,dohc,commo
-00008090: 6e20 7261 696c 2c36 302c 3336 3030 2c38  n rail,60,3600,8
-000080a0: 352c 3137 3530 2c32 3730 2c79 6573 2c34  5,1750,270,yes,4
-000080b0: 2c6d 7076 2c35 2c32 3031 342c 3332 3835  ,mpv,5,2014,3285
-000080c0: 302c 352c 3230 3134 2c61 7574 6f6d 6174  0,5,2014,automat
-000080d0: 6963 2c31 322e 362c 342e 322c 3131 302c  ic,12.6,4.2,110,
-000080e0: 432c 342c 3138 332c 342e 352c 342e 3138  C,4,183,4.5,4.18
-000080f0: 2c32 3435 302c 3133 3938 2c32 3032 302c  ,2450,1398,2020,
-00008100: 3735 2c38 382e 332c 3330 332e 3635 2c33  75,88.3,303.65,3
-00008110: 3138 2e38 3334 3935 3135 2c5b 332e 3534  18.8349515,[3.54
-00008120: 2d20 312e 3932 2d20 312e 3332 2d20 302e  - 1.92- 1.32- 0.
-00008130: 3938 2d20 302e 3736 2d20 302e 365d 2c31  98- 0.76- 0.6],1
-00008140: 3335 372e 352c 3134 3332 2e35 2c31 3435  357.5,1432.5,145
-00008150: 372e 352c 3134 3730 2c33 2e30 3130 3834  7.5,1470,3.01084
-00008160: 332c 4d0d 0a32 3432 3638 2c4d 2c33 3431  3,M..24268,M,341
-00008170: 3034 2c79 6573 2c79 6573 2c79 6573 2c79  04,yes,yes,yes,y
-00008180: 6573 2c2c 7965 732c 7965 732c 7965 732c  es,,yes,yes,yes,
-00008190: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
-000081a0: 7065 7472 6f6c 2c31 3138 2c32 3430 2c66  petrol,118,240,f
-000081b0: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
-000081c0: 2e36 3538 2c34 2e37 3638 2c32 2e38 352c  .658,4.768,2.85,
-000081d0: 312e 3838 342c 2c31 3539 362c 7265 6775  1.884,,1596,regu
-000081e0: 6c61 722c 342c 646f 6863 2c64 6972 6563  lar,4,dohc,direc
-000081f0: 7420 696e 6a65 6374 696f 6e2c 3730 2c35  t injection,70,5
-00008200: 3730 302c 3131 382c 3137 3530 2c32 3430  700,118,1750,240
-00008210: 2c79 6573 2c34 2c6d 7076 2c35 2c61 7661  ,yes,4,mpv,5,ava
-00008220: 696c 6162 6c65 2c33 3938 3835 2c35 2d4a  ilable,39885,5-J
-00008230: 756c 2c32 3031 332c 6d61 6e75 616c 2c39  ul,2013,manual,9
-00008240: 2e38 2c37 2c31 3539 2c43 2c35 2e37 2c32  .8,7,159,C,5.7,2
-00008250: 3034 2c39 2e34 2c34 2e30 372c 2c31 3439  04,9.4,4.07,,149
-00008260: 382c 3234 3030 2c37 352c 3831 2e34 2c33  8,2400,75,81.4,3
-00008270: 3033 2e36 352c 3331 382e 3833 3439 3531  03.65,318.834951
-00008280: 352c 5b33 2e38 2d20 322e 3134 2d20 312e  5,[3.8- 2.14- 1.
-00008290: 3438 2d20 312e 3131 2d20 302e 395d 2c31  48- 1.11- 0.9],1
-000082a0: 3435 302e 3735 2c31 3532 352e 3735 2c31  450.75,1525.75,1
-000082b0: 3535 302e 3735 2c31 3437 302c 332e 3132  550.75,1470,3.12
-000082c0: 3336 3732 2c4d 0d0a 3139 3032 382c 4d2c  3672,M..19028,M,
-000082d0: 3235 3733 342c 7965 732c 7965 732c 7965  25734,yes,yes,ye
-000082e0: 732c 6e6f 2c2c 6e6f 2c6e 6f2c 7965 732c  s,no,,no,no,yes,
-000082f0: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-00008300: 2c70 6574 726f 6c2c 3130 332c 3230 302c  ,petrol,103,200,
-00008310: 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c 2c2c  front,,,,,,,,,,,
-00008320: 312e 3638 352c 342e 3635 382c 322e 3736  1.685,4.658,2.76
-00008330: 2c31 2e38 322c 2c31 3336 342c 7265 6775  ,1.82,,1364,regu
-00008340: 6c61 722c 342c 646f 6863 2c6d 756c 7469  lar,4,dohc,multi
-00008350: 706f 696e 7420 696e 6a65 6374 696f 6e2c  point injection,
-00008360: 3538 2c34 3930 302c 3130 332c 3138 3530  58,4900,103,1850
-00008370: 2c32 3030 2c79 6573 2c34 2c6d 7076 2c35  ,200,yes,4,mpv,5
-00008380: 2c61 7661 696c 6162 6c65 2c32 3831 3935  ,available,28195
-00008390: 2c35 2d4a 756c 2c32 3031 352c 6d61 6e75  ,5-Jul,2015,manu
+00002150: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00002160: 7965 732c 6e6f 2c2c 656c 6563 7472 6963  yes,no,,electric
+00002170: 2065 6e67 696e 652c 656c 6563 7472 6963   engine,electric
+00002180: 6974 792c 3130 372c 3235 302c 6672 6f6e  ity,107,250,fron
+00002190: 742c 3233 2c6c 6974 6869 756d 2d69 6f6e  t,23,lithium-ion
+000021a0: 2c34 3030 2c2c 7065 726d 616e 656e 7420  ,400,,permanent 
+000021b0: 6d61 676e 6574 2073 796e 6368 726f 6e6f  magnet synchrono
+000021c0: 7573 206d 6f74 6f72 2c32 3530 2c31 2c31  us motor,250,1,1
+000021d0: 3037 2c31 3632 2c2c 312e 3436 362c 342e  07,162,,1.466,4.
+000021e0: 3335 382c 322e 3634 382c 312e 3832 332c  358,2.648,1.823,
+000021f0: 2c2c 2c2c 2c2c 2c2c 2c2c 2c2c 2c68 6174  ,,,,,,,,,,,,,hat
+00002200: 6368 6261 636b 2c35 2c32 3031 342c 3339  chback,5,2014,39
+00002210: 3939 302c 352c 3230 3133 2c73 696e 676c  990,5,2013,singl
+00002220: 652d 7370 6565 6420 6669 7865 6420 6765  e-speed fixed ge
+00002230: 6172 2c31 312e 342c 2c30 2c41 2c2c 3133  ar,11.4,,0,A,,13
+00002240: 352c 2c37 2e38 322c 2c31 3634 342c 2c2c  5,,7.82,,1644,,,
+00002250: 2c33 3233 2e34 2c33 3130 2c2c 3136 3434  ,323.4,310,,1644
+00002260: 2c2c 2c2c 322e 3637 3235 3138 2c43 0d0a  ,,,,2.672518,C..
+00002270: 3339 3732 332c 432c 3536 3530 312c 7965  39723,C,56501,ye
+00002280: 732c 7965 732c 7965 732c 7965 732c 2c6e  s,yes,yes,yes,,n
+00002290: 6f2c 7965 732c 7965 732c 7965 732c 2c66  o,yes,yes,yes,,f
+000022a0: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
+000022b0: 6c2c 3936 2c32 3330 2c66 726f 6e74 2c2c  l,96,230,front,,
+000022c0: 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3731 2c34  ,,,,,,,,,1.471,4
+000022d0: 2e35 3835 2c32 2e37 332c 312e 3830 342c  .585,2.73,1.804,
+000022e0: 2c31 3139 392c 7265 6775 6c61 722c 332c  ,1199,regular,3,
+000022f0: 646f 6863 2c6d 756c 7469 706f 696e 7420  dohc,multipoint 
+00002300: 696e 6a65 6374 696f 6e2c 3533 2c35 3530  injection,53,550
+00002310: 302c 3936 2c31 3735 302c 3233 302c 7965  0,96,1750,230,ye
+00002320: 732c 342c 7374 6174 696f 6e77 6167 6f6e  s,4,stationwagon
+00002330: 2c35 2c61 7661 696c 6162 6c65 2c32 3930  ,5,available,290
+00002340: 3130 2c35 2c32 3031 352c 6d61 6e75 616c  10,5,2015,manual
+00002350: 2c31 302c 342e 372c 3130 392c 412c 342c  ,10,4.7,109,A,4,
+00002360: 3230 352c 352e 392c 342e 3138 2c32 3435  205,5.9,4.18,245
+00002370: 302c 3131 3635 2c31 3834 302c 3830 2c39  0,1165,1840,80,9
+00002380: 302e 352c 3239 342e 3837 352c 3330 372e  0.5,294.875,307.
+00002390: 3931 3236 3231 342c 5b33 2e35 342d 2031  9126214,[3.54- 1
+000023a0: 2e39 322d 2031 2e32 322d 2030 2e38 362d  .92- 1.22- 0.86-
+000023b0: 2030 2e37 2d20 302e 3539 5d2c 3131 3239   0.7- 0.59],1129
+000023c0: 2e32 3235 2c31 3230 342e 3232 352c 3132  .225,1204.225,12
+000023d0: 3239 2e32 3235 2c31 3235 302c 322e 3635  29.225,1250,2.65
+000023e0: 3336 3834 2c43 0d0a 3334 3039 322c 432c  3684,C..34092,C,
+000023f0: 3438 3533 352c 7965 732c 7965 732c 7965  48535,yes,yes,ye
+00002400: 732c 7965 732c 2c79 6573 2c79 6573 2c79  s,yes,,yes,yes,y
+00002410: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
+00002420: 696e 652c 6469 6573 656c 2c31 3333 2c34  ine,diesel,133,4
+00002430: 3030 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  00,front,,,,,,,,
+00002440: 2c2c 2c31 2e34 3537 2c34 2e32 3533 2c32  ,,,1.457,4.253,2
+00002450: 2e36 322c 312e 3830 342c 2c31 3939 372c  .62,1.804,,1997,
+00002460: 7061 7274 6963 6c65 2066 696c 7465 722c  particle filter,
+00002470: 342c 646f 6863 2c63 6f6d 6d6f 6e20 7261  4,dohc,common ra
+00002480: 696c 2c35 332c 3337 3530 2c31 3333 2c32  il,53,3750,133,2
+00002490: 3030 302c 3430 302c 7965 732c 342c 6861  000,400,yes,4,ha
+000024a0: 7463 6862 6163 6b2c 352c 6176 6169 6c61  tchback,5,availa
+000024b0: 626c 652c 3335 3333 302c 352c 3230 3135  ble,35330,5,2015
+000024c0: 2c61 7574 6f6d 6174 6963 2c38 2e34 2c34  ,automatic,8.4,4
+000024d0: 2c31 3033 2c43 2c33 2e35 2c32 3230 2c34  ,103,C,3.5,220,4
+000024e0: 2e37 2c32 2e39 352c 3139 3530 2c31 3239  .7,2.95,1950,129
+000024f0: 352c 3139 3230 2c2c 3838 2c32 3938 2e38  5,1920,,88,298.8
+00002500: 2c33 3039 2e33 3230 3338 3833 2c5b 342e  ,309.3203883,[4.
+00002510: 3435 2d20 322e 352d 2031 2e35 362d 2031  45- 2.5- 1.56- 1
+00002520: 2e31 342d 2030 2e38 352d 2030 2e36 375d  .14- 0.85- 0.67]
+00002530: 2c31 3235 392e 3232 352c 3133 3334 2e32  ,1259.225,1334.2
+00002540: 3235 2c31 3335 392e 3232 352c 3133 3630  25,1359.225,1360
+00002550: 2c32 2e36 3238 3432 382c 430d 0a32 3539  ,2.628428,C..259
+00002560: 322c 432c 3335 3634 2c79 6573 2c79 6573  2,C,3564,yes,yes
+00002570: 2c79 6573 2c79 6573 2c2c 7965 732c 3536  ,yes,yes,,yes,56
+00002580: 302c 7965 732c 7965 732c 2c66 7565 6c20  0,yes,yes,,fuel 
+00002590: 656e 6769 6e65 2c64 6965 7365 6c2c 3831  engine,diesel,81
+000025a0: 2c32 3530 2c66 726f 6e74 2c2c 2c2c 2c2c  ,250,front,,,,,,
+000025b0: 2c2c 2c2c 2c31 2e34 3231 2c34 2e32 3337  ,,,,,1.421,4.237
+000025c0: 2c32 2e36 3031 2c31 2e37 3737 2c2c 3135  ,2.601,1.777,,15
+000025d0: 3938 2c70 6172 7469 636c 6520 6669 6c74  98,particle filt
+000025e0: 6572 2c34 2c64 6f68 632c 636f 6d6d 6f6e  er,4,dohc,common
+000025f0: 2072 6169 6c2c 3530 2c33 3230 302c 3831   rail,50,3200,81
+00002600: 2c31 3530 302c 3235 302c 7965 732c 342c  ,1500,250,yes,4,
+00002610: 6861 7463 6862 6163 6b2c 332c 6176 6169  hatchback,3,avai
+00002620: 6c61 626c 652c 3333 3734 302c 352c 3230  lable,33740,5,20
+00002630: 3134 2c6d 616e 7561 6c2c 3130 2e35 2c33  14,manual,10.5,3
+00002640: 2e38 2c39 392c 432c 332e 342c 3230 302c  .8,99,C,3.4,200,
+00002650: 342e 352c 332e 3339 2c32 3030 302c 3132  4.5,3.39,2000,12
+00002660: 3035 2c31 3739 302c 3735 2c38 302e 352c  05,1790,75,80.5,
+00002670: 3239 342e 3837 352c 3330 372e 3931 3236  294.875,307.9126
+00002680: 3231 342c 5b34 2e31 312d 2032 2e31 322d  214,[4.11- 2.12-
+00002690: 2031 2e33 362d 2030 2e39 372d 2030 2e37   1.36- 0.97- 0.7
+000026a0: 332d 2030 2e35 395d 2c31 3137 312e 3235  3- 0.59],1171.25
+000026b0: 2c31 3234 362e 3235 2c31 3237 312e 3235  ,1246.25,1271.25
+000026c0: 2c31 3235 302c 322e 3532 3531 3137 2c43  ,1250,2.525117,C
+000026d0: 0d0a 3536 3335 2c43 2c36 3931 312c 7965  ..5635,C,6911,ye
+000026e0: 732c 7965 732c 7965 732c 6e6f 2c2c 6e6f  s,yes,yes,no,,no
+000026f0: 2c6e 6f2c 7965 732c 6e6f 2c2c 6675 656c  ,no,yes,no,,fuel
+00002700: 2065 6e67 696e 652c 7065 7472 6f6c 2c38   engine,petrol,8
+00002710: 312c 3230 352c 6672 6f6e 742c 2c2c 2c2c  1,205,front,,,,,
+00002720: 2c2c 2c2c 2c2c 312e 3438 392c 342e 3332  ,,,,,,1.489,4.32
+00002730: 392c 322e 3630 382c 312e 3738 392c 2c31  9,2.608,1.789,,1
+00002740: 3139 392c 7265 6775 6c61 722c 332c 646f  199,regular,3,do
+00002750: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
+00002760: 696f 6e2c 3630 2c35 3530 302c 3831 2c31  ion,60,5500,81,1
+00002770: 3735 302c 3230 352c 7965 732c 342c 6861  750,205,yes,4,ha
+00002780: 7463 6862 6163 6b2c 352c 6176 6169 6c61  tchback,5,availa
+00002790: 626c 652c 3139 3739 302c 352c 3230 3135  ble,19790,5,2015
+000027a0: 2c6d 616e 7561 6c2c 3132 2e33 2c34 2e38  ,manual,12.3,4.8
+000027b0: 2c31 3132 2c41 2c34 2c31 3834 2c36 2e31  ,112,A,4,184,6.1
+000027c0: 2c34 2e39 332c 3337 3030 2c31 3137 352c  ,4.93,3700,1175,
+000027d0: 3137 3730 2c37 352c 3930 2e35 2c32 3839  1770,75,90.5,289
+000027e0: 2e33 3635 2c33 3038 2e30 3039 3730 3837  .365,308.0097087
+000027f0: 2c5b 332e 3436 2d20 312e 3837 2d20 312e  ,[3.46- 1.87- 1.
+00002800: 3239 2d20 302e 3935 2d20 302e 3735 5d2c  29- 0.95- 0.75],
+00002810: 3131 3334 2e35 2c31 3230 392e 352c 3132  1134.5,1209.5,12
+00002820: 3334 2e35 2c31 3235 302c 322e 3636 3338  34.5,1250,2.6638
+00002830: 3231 2c43 0d0a 3536 3330 2c43 2c36 3930  21,C..5630,C,690
+00002840: 342c 7965 732c 7965 732c 7965 732c 7965  4,yes,yes,yes,ye
+00002850: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
+00002860: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
+00002870: 6965 7365 6c2c 3838 2c33 3030 2c66 726f  iesel,88,300,fro
+00002880: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  nt,,,,,,,,,,,1.4
+00002890: 3839 2c34 2e33 3239 2c32 2e36 3038 2c31  89,4.329,2.608,1
+000028a0: 2e37 3839 2c2c 3135 3630 2c70 6172 7469  .789,,1560,parti
+000028b0: 636c 6520 6669 6c74 6572 2c34 2c64 6f68  cle filter,4,doh
+000028c0: 632c 636f 6d6d 6f6e 2072 6169 6c2c 3630  c,common rail,60
+000028d0: 2c33 3530 302c 3838 2c31 3735 302c 3330  ,3500,88,1750,30
+000028e0: 302c 7965 732c 322c 6861 7463 6862 6163  0,yes,2,hatchbac
+000028f0: 6b2c 352c 6176 6169 6c61 626c 652c 3236  k,5,available,26
+00002900: 3339 302c 352c 3230 3135 2c6d 616e 7561  390,5,2015,manua
+00002910: 6c2c 3130 2e36 2c33 2e36 2c39 332c 422c  l,10.6,3.6,93,B,
+00002920: 332e 332c 3139 372c 342e 312c 332e 3734  3.3,197,4.1,3.74
+00002930: 2c32 3130 302c 3132 3535 2c31 3836 302c  ,2100,1255,1860,
+00002940: 3535 2c38 382e 332c 3239 312e 3134 352c  55,88.3,291.145,
+00002950: 3330 362e 3734 3735 3732 382c 5b33 2e35  306.7475728,[3.5
+00002960: 342d 2031 2e39 322d 2031 2e32 382d 2030  4- 1.92- 1.28- 0
+00002970: 2e39 312d 2030 2e36 372d 2030 2e35 365d  .91- 0.67- 0.56]
+00002980: 2c31 3231 342e 352c 3132 3839 2e35 2c31  ,1214.5,1289.5,1
+00002990: 3331 342e 352c 3132 3530 2c32 2e36 3633  314.5,1250,2.663
+000029a0: 3832 312c 430d 0a37 3636 312c 432c 3931  821,C..7661,C,91
+000029b0: 3933 2c79 6573 2c79 6573 2c79 6573 2c6e  93,yes,yes,yes,n
+000029c0: 6f2c 2c6e 6f2c 3339 352c 7965 732c 6e6f  o,,no,395,yes,no
+000029d0: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
+000029e0: 7472 6f6c 2c31 3235 2c32 3630 2c66 726f  trol,125,260,fro
+000029f0: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35  nt,,,,,,,,,,,1.5
+00002a00: 312c 342e 3431 392c 322e 3638 352c 312e  1,4.419,2.685,1.
+00002a10: 3831 342c 2c31 3539 382c 7265 6775 6c61  814,,1598,regula
+00002a20: 722c 342c 646f 6863 2c64 6972 6563 7420  r,4,dohc,direct 
+00002a30: 696e 6a65 6374 696f 6e2c 3536 2c36 3030  injection,56,600
+00002a40: 302c 3132 352c 3136 3530 2c32 3630 2c79  0,125,1650,260,y
+00002a50: 6573 2c34 2c68 6174 6368 6261 636b 2c35  es,4,hatchback,5
+00002a60: 2c61 7661 696c 6162 6c65 2c32 3638 3435  ,available,26845
+00002a70: 2c35 2c32 3031 352c 6d61 6e75 616c 2c38  ,5,2015,manual,8
+00002a80: 2e37 2c35 2e39 2c31 3339 2c43 2c34 2e39  .7,5.9,139,C,4.9
+00002a90: 2c32 3230 2c37 2e38 2c33 2e38 332c 3237  ,220,7.8,3.83,27
+00002aa0: 3530 2c31 3333 302c 3230 3030 2c37 352c  50,1330,2000,75,
+00002ab0: 3831 2e35 2c33 3033 2e36 352c 3331 382e  81.5,303.65,318.
+00002ac0: 3833 3439 3531 352c 5b33 2e38 322d 2032  8349515,[3.82- 2
+00002ad0: 2e31 362d 2031 2e34 382d 2031 2e30 372d  .16- 1.48- 1.07-
+00002ae0: 2030 2e38 382d 2030 2e37 345d 2c31 3239   0.88- 0.74],129
+00002af0: 322e 322c 3133 3637 2e32 2c31 3339 322e  2.2,1367.2,1392.
+00002b00: 322c 3133 3630 2c32 2e37 3339 3134 2c43  2,1360,2.73914,C
+00002b10: 0d0a 3736 3833 2c43 2c39 3231 352c 7965  ..7683,C,9215,ye
+00002b20: 732c 7965 732c 7965 732c 6e6f 2c2c 6e6f  s,yes,yes,no,,no
+00002b30: 2c33 3935 2c79 6573 2c79 6573 2c2c 6675  ,395,yes,yes,,fu
+00002b40: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
+00002b50: 2c31 3231 2c33 3530 2c66 726f 6e74 2c2c  ,121,350,front,,
+00002b60: 2c2c 2c2c 2c2c 2c2c 2c31 2e35 312c 342e  ,,,,,,,,,1.51,4.
+00002b70: 3431 392c 322e 3638 352c 312e 3831 342c  419,2.685,1.814,
+00002b80: 2c31 3935 362c 7061 7274 6963 6c65 2066  ,1956,particle f
+00002b90: 696c 7465 722c 342c 6f68 632c 636f 6d6d  ilter,4,ohc,comm
+00002ba0: 6f6e 2072 6169 6c2c 3536 2c34 3030 302c  on rail,56,4000,
+00002bb0: 3132 312c 3137 3530 2c33 3530 2c79 6573  121,1750,350,yes
+00002bc0: 2c34 2c68 6174 6368 6261 636b 2c35 2c61  ,4,hatchback,5,a
+00002bd0: 7661 696c 6162 6c65 2c32 3934 3935 2c35  vailable,29495,5
+00002be0: 2c32 3031 352c 6d61 6e75 616c 2c39 2c34  ,2015,manual,9,4
+00002bf0: 2e35 2c31 3139 2c44 2c34 2c32 3135 2c35  .5,119,D,4,215,5
+00002c00: 2e34 2c33 2e33 352c 3230 3030 2c31 3431  .4,3.35,2000,141
+00002c10: 382c 3230 3430 2c37 352c 3930 2e34 2c33  8,2040,75,90.4,3
+00002c20: 3033 2e36 352c 3331 382e 3833 3439 3531  03.65,318.834951
+00002c30: 352c 5b34 2e31 372d 2032 2e31 332d 2031  5,[4.17- 2.13- 1
+00002c40: 2e33 322d 2030 2e39 352d 2030 2e37 352d  .32- 0.95- 0.75-
+00002c50: 2030 2e36 325d 2c31 3338 302e 322c 3134   0.62],1380.2,14
+00002c60: 3535 2e32 2c31 3438 302e 322c 3134 3730  55.2,1480.2,1470
+00002c70: 2c32 2e37 3339 3134 2c43 0d0a 3837 3039  ,2.73914,C..8709
+00002c80: 2c43 2c31 3038 3330 2c79 6573 2c79 6573  ,C,10830,yes,yes
+00002c90: 2c6e 6f2c 6e6f 2c2c 6e6f 2c6e 6f2c 7965  ,no,no,,no,no,ye
+00002ca0: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
+00002cb0: 6e65 2c70 6574 726f 6c2c 3939 2c31 3634  ne,petrol,99,164
+00002cc0: 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c  ,front,,,,,,,,,,
+00002cd0: 2c31 2e34 3635 2c34 2e33 2c32 2e36 352c  ,1.465,4.3,2.65,
+00002ce0: 312e 3738 2c2c 3135 3931 2c72 6567 756c  1.78,,1591,regul
+00002cf0: 6172 2c34 2c64 6f68 632c 6469 7265 6374  ar,4,dohc,direct
+00002d00: 2069 6e6a 6563 7469 6f6e 2c35 332c 3633   injection,53,63
+00002d10: 3030 2c39 392c 3438 3530 2c31 3634 2c6e  00,99,4850,164,n
+00002d20: 6f2c 342c 6861 7463 6862 6163 6b2c 352c  o,4,hatchback,5,
+00002d30: 6176 6169 6c61 626c 652c 3139 3939 352c  available,19995,
+00002d40: 352c 3230 3134 2c6d 616e 7561 6c2c 392e  5,2014,manual,9.
+00002d50: 392c 352c 3131 382c 422c 342e 332c 3139  9,5,118,B,4.3,19
+00002d60: 302c 362e 342c 342e 3036 2c32 3830 302c  0,6.4,4.06,2800,
+00002d70: 3131 3638 2c31 3732 302c 3830 2c38 352e  1168,1720,80,85.
+00002d80: 342c 3238 392e 3336 352c 3330 382e 3030  4,289.365,308.00
+00002d90: 3937 3038 372c 5b33 2e37 372d 2032 2e30  97087,[3.77- 2.0
+00002da0: 352d 2031 2e33 372d 2031 2e30 342d 2030  5- 1.37- 1.04- 0
+00002db0: 2e38 342d 2030 2e36 395d 2c31 3133 322e  .84- 0.69],1132.
+00002dc0: 3232 352c 3132 3037 2e32 3235 2c31 3233  225,1207.225,123
+00002dd0: 322e 3232 352c 3132 3530 2c32 2e36 3037  2.225,1250,2.607
+00002de0: 372c 430d 0a39 3736 392c 432c 3132 3037  7,C..9769,C,1207
+00002df0: 322c 7965 732c 7965 732c 7965 732c 7965  2,yes,yes,yes,ye
+00002e00: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
+00002e10: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
+00002e20: 6965 7365 6c2c 3934 2c32 3630 2c66 726f  iesel,94,260,fro
+00002e30: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  nt,,,,,,,,,,,1.4
+00002e40: 3635 2c34 2e33 2c32 2e36 352c 312e 3738  65,4.3,2.65,1.78
+00002e50: 2c2c 3135 3832 2c70 6172 7469 636c 6520  ,,1582,particle 
+00002e60: 6669 6c74 6572 2c34 2c64 6f68 632c 636f  filter,4,dohc,co
+00002e70: 6d6d 6f6e 2072 6169 6c2c 3533 2c34 3030  mmon rail,53,400
+00002e80: 302c 3934 2c31 3930 302c 3236 302c 7965  0,94,1900,260,ye
+00002e90: 732c 342c 6861 7463 6862 6163 6b2c 332c  s,4,hatchback,3,
+00002ea0: 3230 3134 2c32 3537 3935 2c35 2c32 3031  2014,25795,5,201
+00002eb0: 332c 6d61 6e75 616c 2c31 302e 392c 332e  3,manual,10.9,3.
+00002ec0: 372c 3937 2c43 2c33 2e35 2c31 3838 2c34  7,97,C,3.5,188,4
+00002ed0: 2e31 2c33 2e34 372c 3231 3030 2c31 3236  .1,3.47,2100,126
+00002ee0: 352c 3138 3130 2c38 302c 3835 2c32 3931  5,1810,80,85,291
+00002ef0: 2e31 3435 2c33 3036 2e37 3437 3537 3238  .145,306.7475728
+00002f00: 2c5b 332e 3737 2d20 322e 3035 2d20 312e  ,[3.77- 2.05- 1.
+00002f10: 3139 2d20 302e 3834 2d20 302e 372d 2030  19- 0.84- 0.7- 0
+00002f20: 2e36 5d2c 3132 3239 2e32 3235 2c31 3330  .6],1229.225,130
+00002f30: 342e 3232 352c 3133 3239 2e32 3235 2c31  4.225,1329.225,1
+00002f40: 3235 302c 322e 3630 3737 2c43 0d0a 3138  250,2.6077,C..18
+00002f50: 3732 2c43 2c32 3833 342c 7965 732c 7965  72,C,2834,yes,ye
+00002f60: 732c 7965 732c 7965 732c 2c6e 6f2c 7965  s,yes,yes,,no,ye
+00002f70: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
+00002f80: 656e 6769 6e65 2c64 6965 7365 6c2c 3838  engine,diesel,88
+00002f90: 2c32 3830 2c66 726f 6e74 2c2c 2c2c 2c2c  ,280,front,,,,,,
+00002fa0: 2c2c 2c2c 2c31 2e34 372c 342e 3337 2c32  ,,,,,1.47,4.37,2
+00002fb0: 2e36 3436 2c31 2e38 3032 2c2c 3139 3639  .646,1.802,,1969
+00002fc0: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
+00002fd0: 2c34 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,4,dohc,common r
+00002fe0: 6169 6c2c 3532 2c33 3735 302c 3838 2c31  ail,52,3750,88,1
+00002ff0: 3530 302c 3238 302c 7965 732c 342c 6861  500,280,yes,4,ha
+00003000: 7463 6862 6163 6b2c 352c 6176 6169 6c61  tchback,5,availa
+00003010: 626c 652c 3337 3939 352c 352c 3230 3135  ble,37995,5,2015
+00003020: 2c6d 616e 7561 6c2c 3130 2e36 2c33 2e37  ,manual,10.6,3.7
+00003030: 2c39 362c 422c 332e 342c 3139 302c 342e  ,96,B,3.4,190,4.
+00003040: 322c 332e 3631 2c32 3135 302c 3133 3438  2,3.61,2150,1348
+00003050: 2c31 3938 302c 3130 302c 3933 2e32 2c33  ,1980,100,93.2,3
+00003060: 3033 2e36 352c 3331 382e 3833 3439 3531  03.65,318.834951
+00003070: 352c 5b33 2e37 332d 2032 2e30 352d 2031  5,[3.73- 2.05- 1
+00003080: 2e32 362d 2030 2e39 322d 2030 2e37 342d  .26- 0.92- 0.74-
+00003090: 2030 2e36 325d 2c31 3331 322e 392c 3133   0.62],1312.9,13
+000030a0: 3837 2e39 2c31 3431 322e 392c 3133 3630  87.9,1412.9,1360
+000030b0: 2c32 2e36 3438 3934 2c43 0d0a 3130 3332  ,2.64894,C..1032
+000030c0: 382c 432c 3133 3536 322c 7965 732c 7965  8,C,13562,yes,ye
+000030d0: 732c 7965 732c 7965 732c 2c6e 6f2c 7965  s,yes,yes,,no,ye
+000030e0: 732c 7965 732c 6e6f 2c2c 6675 656c 2065  s,yes,no,,fuel e
+000030f0: 6e67 696e 652c 7065 7472 6f6c 2c31 3037  ngine,petrol,107
+00003100: 2c31 3835 2c66 726f 6e74 2c2c 2c2c 2c2c  ,185,front,,,,,,
+00003110: 2c2c 2c2c 2c31 2e34 3537 2c34 2e35 3232  ,,,,,1.457,4.522
+00003120: 2c32 2e36 342c 312e 3737 2c2c 3139 3939  ,2.64,1.77,,1999
+00003130: 2c72 6567 756c 6172 2c34 2c64 6f68 632c  ,regular,4,dohc,
+00003140: 6d75 6c74 6970 6f69 6e74 2069 6e6a 6563  multipoint injec
+00003150: 7469 6f6e 2c35 352c 3630 3030 2c31 3037  tion,55,6000,107
+00003160: 2c34 3030 302c 3138 352c 6e6f 2c34 2c73  ,4000,185,no,4,s
+00003170: 7461 7469 6f6e 7761 676f 6e2c 352c 3230  tationwagon,5,20
+00003180: 3132 2c33 3137 3530 2c35 2c32 3031 312c  12,31750,5,2011,
+00003190: 6d61 6e75 616c 2c39 2e36 2c37 2e36 2c31  manual,9.6,7.6,1
+000031a0: 3736 2c46 2c35 2e37 2c32 3130 2c31 302e  76,F,5.7,210,10.
+000031b0: 382c 342e 3037 2c33 3530 302c 3132 3833  8,4.07,3500,1283
+000031c0: 2c31 3839 302c 3130 302c 3833 2e31 2c32  ,1890,100,83.1,2
+000031d0: 3931 2e31 3435 2c33 3036 2e37 3437 3537  91.145,306.74757
+000031e0: 3238 2c5b 332e 3432 2d20 322e 3134 2d20  28,[3.42- 2.14- 
+000031f0: 312e 3438 2d20 312e 3131 2d20 302e 3835  1.48- 1.11- 0.85
+00003200: 5d2c 3132 3435 2e38 3735 2c31 3332 302e  ],1245.875,1320.
+00003210: 3837 352c 3133 3435 2e38 3735 2c31 3336  875,1345.875,136
+00003220: 302c 322e 3537 3838 392c 430d 0a33 3534  0,2.57889,C..354
+00003230: 3736 2c44 2c35 3033 3536 2c79 6573 2c79  76,D,50356,yes,y
+00003240: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
+00003250: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00003260: 2065 6e67 696e 652c 7065 7472 6f6c 2c39   engine,petrol,9
+00003270: 322c 3230 302c 6672 6f6e 742c 2c2c 2c2c  2,200,front,,,,,
+00003280: 2c2c 2c2c 2c2c 312e 3436 312c 342e 3736  ,,,,,,1.461,4.76
+00003290: 372c 322e 3739 312c 312e 3833 322c 2c31  7,2.791,1.832,,1
+000032a0: 3339 352c 7265 6775 6c61 722c 342c 646f  395,regular,4,do
+000032b0: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
+000032c0: 696f 6e2c 3636 2c35 3030 302c 3932 2c31  ion,66,5000,92,1
+000032d0: 3430 302c 3230 302c 7965 732c 342c 7365  400,200,yes,4,se
+000032e0: 6461 6e2c 342c 6176 6169 6c61 626c 652c  dan,4,available,
+000032f0: 3332 3335 302c 352c 3230 3135 2c6d 616e  32350,5,2015,man
+00003300: 7561 6c2c 392e 372c 352e 332c 3132 332c  ual,9.7,5.3,123,
+00003310: 412c 342e 342c 3230 382c 362e 382c 342e  A,4.4,208,6.8,4.
+00003320: 3335 2c32 3730 302c 3132 3637 2c31 3931  35,2700,1267,191
+00003330: 302c 3130 302c 3830 2c33 3033 2e38 322c  0,100,80,303.82,
+00003340: 3332 322e 3532 3432 3731 382c 5b33 2e36  322.5242718,[3.6
+00003350: 322d 2031 2e39 352d 2031 2e32 382d 2030  2- 1.95- 1.28- 0
+00003360: 2e39 372d 2030 2e37 382d 2030 2e36 355d  .97- 0.78- 0.65]
+00003370: 2c31 3232 322e 3435 2c31 3239 372e 3435  ,1222.45,1297.45
+00003380: 2c31 3332 322e 3435 2c31 3235 302c 322e  ,1322.45,1250,2.
+00003390: 3637 3635 3532 2c44 0d0a 3431 3938 392c  676552,D..41989,
+000033a0: 442c 3539 3639 372c 7965 732c 7965 732c  D,59697,yes,yes,
+000033b0: 7965 732c 7965 732c 2c6e 6f2c 7965 732c  yes,yes,,no,yes,
+000033c0: 7965 732c 7965 732c 2c66 7565 6c20 656e  yes,yes,,fuel en
+000033d0: 6769 6e65 2c64 6965 7365 6c2c 3838 2c32  gine,diesel,88,2
+000033e0: 3530 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  50,front,,,,,,,,
+000033f0: 2c2c 2c31 2e34 3631 2c34 2e37 3637 2c32  ,,,1.461,4.767,2
+00003400: 2e37 3931 2c31 2e38 3332 2c2c 3135 3938  .791,1.832,,1598
+00003410: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
+00003420: 2c34 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,4,dohc,common r
+00003430: 6169 6c2c 3636 2c33 3630 302c 3838 2c31  ail,66,3600,88,1
+00003440: 3530 302c 3235 302c 7965 732c 342c 7365  500,250,yes,4,se
+00003450: 6461 6e2c 342c 6176 6169 6c61 626c 652c  dan,4,available,
+00003460: 3334 3835 302c 352c 3230 3135 2c6d 616e  34850,5,2015,man
+00003470: 7561 6c2c 3130 2e38 2c34 2c31 3038 2c42  ual,10.8,4,108,B
+00003480: 2c33 2e36 2c32 3036 2c34 2e37 2c33 2e36  ,3.6,206,4.7,3.6
+00003490: 352c 3230 3530 2c31 3334 342c 3139 3930  5,2050,1344,1990
+000034a0: 2c31 3030 2c38 302e 352c 3330 332e 3832  ,100,80.5,303.82
+000034b0: 2c33 3232 2e35 3234 3237 3138 2c5b 342e  ,322.5242718,[4.
+000034c0: 3131 2d20 322e 3132 2d20 312e 3336 2d20  11- 2.12- 1.36- 
+000034d0: 302e 3937 2d20 302e 3733 2d20 302e 3539  0.97- 0.73- 0.59
+000034e0: 5d2c 3132 3939 2e34 352c 3133 3734 2e34  ],1299.45,1374.4
+000034f0: 352c 3133 3939 2e34 352c 3133 3630 2c32  5,1399.45,1360,2
+00003500: 2e36 3736 3535 322c 440d 0a32 3637 3939  .676552,D..26799
+00003510: 2c44 2c33 3738 3534 2c79 6573 2c79 6573  ,D,37854,yes,yes
+00003520: 2c79 6573 2c79 6573 2c2c 6e6f 2c79 6573  ,yes,yes,,no,yes
+00003530: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+00003540: 6e67 696e 652c 7065 7472 6f6c 2c31 3235  ngine,petrol,125
+00003550: 2c33 3230 2c66 726f 6e74 2b72 6561 722c  ,320,front+rear,
+00003560: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3432 372c  ,,,,,,,,,,1.427,
+00003570: 342e 3730 312c 322e 3830 382c 312e 3832  4.701,2.808,1.82
+00003580: 362c 2c31 3739 382c 7265 6775 6c61 722c  6,,1798,regular,
+00003590: 342c 646f 6863 2c64 6972 6563 7420 696e  4,dohc,direct in
+000035a0: 6a65 6374 696f 6e2c 3631 2c33 3830 302c  jection,61,3800,
+000035b0: 3132 352c 3134 3030 2c33 3230 2c79 6573  125,1400,320,yes
+000035c0: 2c34 2c73 6564 616e 2c34 2c61 7661 696c  ,4,sedan,4,avail
+000035d0: 6162 6c65 2c34 3130 3235 2c35 2c32 3031  able,41025,5,201
+000035e0: 352c 6d61 6e75 616c 2c37 2e39 2c36 2e32  5,manual,7.9,6.2
+000035f0: 2c31 3334 2c42 2c35 2e32 2c32 3239 2c38  ,134,B,5.2,229,8
+00003600: 2e31 2c33 2e36 392c 3232 3530 2c31 3438  .1,3.69,2250,148
+00003610: 302c 3139 3830 2c39 302c 3834 2e31 2c32  0,1980,90,84.1,2
+00003620: 3939 2e37 3235 2c33 3137 2e34 3237 3138  99.725,317.42718
+00003630: 3435 2c5b 332e 3738 2d20 322e 3035 2d20  45,[3.78- 2.05- 
+00003640: 312e 3332 2d20 302e 3937 2d20 302e 3736  1.32- 0.97- 0.76
+00003650: 2d20 302e 3633 5d2c 3134 3338 2e38 3235  - 0.63],1438.825
+00003660: 2c31 3531 332e 3832 352c 3135 3338 2e38  ,1513.825,1538.8
+00003670: 3235 2c31 3437 302c 322e 3630 3537 3032  25,1470,2.605702
+00003680: 2c44 0d0a 3236 3835 312c 442c 3337 3932  ,D..26851,D,3792
+00003690: 362c 7965 732c 7965 732c 7965 732c 7965  6,yes,yes,yes,ye
+000036a0: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
+000036b0: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
+000036c0: 6965 7365 6c2c 3134 302c 3430 302c 6672  iesel,140,400,fr
+000036d0: 6f6e 742b 7265 6172 2c2c 2c2c 2c2c 2c2c  ont+rear,,,,,,,,
+000036e0: 2c2c 2c31 2e34 3237 2c34 2e37 3031 2c32  ,,,1.427,4.701,2
+000036f0: 2e38 3038 2c31 2e38 3236 2c2c 3139 3638  .808,1.826,,1968
+00003700: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
+00003710: 2c34 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,4,dohc,common r
+00003720: 6169 6c2c 3633 2c34 3230 302c 3134 302c  ail,63,4200,140,
+00003730: 3137 3530 2c34 3030 2c79 6573 2c34 2c73  1750,400,yes,4,s
+00003740: 6564 616e 2c34 2c61 7661 696c 6162 6c65  edan,4,available
+00003750: 2c35 3334 3530 2c35 2c32 3031 342c 6175  ,53450,5,2014,au
+00003760: 746f 6d61 7469 632c 372e 332c 352c 3133  tomatic,7.3,5,13
+00003770: 322c 442c 342e 352c 3233 352c 352e 392c  2,D,4.5,235,5.9,
+00003780: 342e 3039 2c31 3835 302c 3136 3330 2c32  4.09,1850,1630,2
+00003790: 3230 352c 3930 2c39 352e 352c 3330 352e  205,90,95.5,305.
+000037a0: 3034 2c33 3137 2e30 3837 3337 3836 2c5b  04,317.0873786,[
+000037b0: 332e 3639 2d20 322e 3135 2d20 312e 3334  3.69- 2.15- 1.34
+000037c0: 2d20 302e 3937 2d20 302e 3734 2d20 302e  - 0.97- 0.74- 0.
+000037d0: 3537 2d20 302e 3436 5d2c 3135 3837 2e34  57- 0.46],1587.4
+000037e0: 3735 2c31 3636 322e 3437 352c 3136 3837  75,1662.475,1687
+000037f0: 2e34 3735 2c31 3730 302c 322e 3630 3537  .475,1700,2.6057
+00003800: 3032 2c44 0d0a 3237 3138 392c 442c 3338  02,D..27189,D,38
+00003810: 3434 372c 7965 732c 7965 732c 7965 732c  447,yes,yes,yes,
+00003820: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
+00003830: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00003840: 2c70 6574 726f 6c2c 3136 352c 3335 302c  ,petrol,165,350,
+00003850: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
+00003860: 2c2c 2c2c 2c31 2e33 3931 2c34 2e37 3132  ,,,,,1.391,4.712
+00003870: 2c32 2e38 312c 312e 3835 342c 2c31 3938  ,2.81,1.854,,198
+00003880: 342c 7265 6775 6c61 722c 342c 646f 6863  4,regular,4,dohc
+00003890: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
+000038a0: 6e2c 3634 2c34 3530 302c 3136 352c 3135  n,64,4500,165,15
+000038b0: 3030 2c33 3530 2c79 6573 2c34 2c68 6174  00,350,yes,4,hat
+000038c0: 6368 6261 636b 2c35 2c61 7661 696c 6162  chback,5,availab
+000038d0: 6c65 2c35 3630 3230 2c34 2c32 3031 342c  le,56020,4,2014,
+000038e0: 6175 746f 6d61 7469 632c 362e 352c 362e  automatic,6.5,6.
+000038f0: 372c 3135 352c 432c 352e 362c 3234 352c  7,155,C,5.6,245,
+00003900: 382e 352c 342e 3039 2c32 3035 302c 3135  8.5,4.09,2050,15
+00003910: 3930 2c32 3136 352c 3930 2c39 322e 382c  90,2165,90,92.8,
+00003920: 3330 332e 3635 2c33 3138 2e38 3334 3935  303.65,318.83495
+00003930: 3135 2c5b 332e 3639 2d20 322e 3135 2d20  15,[3.69- 2.15- 
+00003940: 312e 3431 2d20 312e 3033 2d20 302e 3739  1.41- 1.03- 0.79
+00003950: 2d20 302e 3633 2d20 302e 3532 5d2c 3135  - 0.63- 0.52],15
+00003960: 3436 2e38 2c31 3632 312e 382c 3136 3436  46.8,1621.8,1646
+00003970: 2e38 2c31 3539 302c 322e 3537 3839 3134  .8,1590,2.578914
+00003980: 2c44 0d0a 3233 3830 312c 442c 3332 3836  ,D..23801,D,3286
+00003990: 362c 7965 732c 7965 732c 7965 732c 7965  6,yes,yes,yes,ye
+000039a0: 732c 2c6e 6f2c 7965 732c 7965 732c 6e6f  s,,no,yes,yes,no
+000039b0: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
+000039c0: 7472 6f6c 2c31 3235 2c32 3130 2c72 6561  trol,125,210,rea
+000039d0: 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3338  r,,,,,,,,,,,1.38
+000039e0: 342c 342e 3631 322c 322e 3736 2c31 2e37  4,4.612,2.76,1.7
+000039f0: 3832 2c2c 3139 3935 2c72 6567 756c 6172  82,,1995,regular
+00003a00: 2c34 2c64 6f68 632c 6469 7265 6374 2069  ,4,dohc,direct i
+00003a10: 6e6a 6563 7469 6f6e 2c36 332c 3637 3030  njection,63,6700
+00003a20: 2c31 3235 2c34 3235 302c 3231 302c 6e6f  ,125,4250,210,no
+00003a30: 2c34 2c63 6162 7269 6f6c 6574 2c32 2c32  ,4,cabriolet,2,2
+00003a40: 3031 332c 3537 3637 322c 342c 3230 3133  013,57672,4,2013
+00003a50: 2c61 7574 6f6d 6174 6963 2c39 2e38 2c37  ,automatic,9.8,7
+00003a60: 2e33 2c31 3639 2c45 2c35 2e38 2c32 3236  .3,169,E,5.8,226
+00003a70: 2c39 2e38 2c34 2e31 2c32 3830 302c 3136  ,9.8,4.1,2800,16
+00003a80: 3030 2c32 3035 352c 2c39 302c 3239 382e  00,2055,,90,298.
+00003a90: 382c 3330 392e 3332 3033 3838 332c 5b34  8,309.3203883,[4
+00003aa0: 2e31 372d 2032 2e33 342d 2031 2e35 322d  .17- 2.34- 1.52-
+00003ab0: 2031 2e31 342d 2030 2e38 362d 2030 2e36   1.14- 0.86- 0.6
+00003ac0: 395d 2c31 3535 372e 3437 352c 3136 3332  9],1557.475,1632
+00003ad0: 2e34 3735 2c31 3635 372e 3437 352c 3135  .475,1657.475,15
+00003ae0: 3930 2c32 2e34 3636 3238 382c 440d 0a33  90,2.466288,D..3
+00003af0: 3037 392c 442c 3430 3635 2c79 6573 2c79  079,D,4065,yes,y
+00003b00: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
+00003b10: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00003b20: 2065 6e67 696e 652c 6469 6573 656c 2c38   engine,diesel,8
+00003b30: 352c 3237 302c 7265 6172 2c2c 2c2c 2c2c  5,270,rear,,,,,,
+00003b40: 2c2c 2c2c 2c31 2e34 3239 2c34 2e36 3234  ,,,,,1.429,4.624
+00003b50: 2c32 2e38 312c 312e 3831 312c 2c31 3939  ,2.81,1.811,,199
+00003b60: 352c 7061 7274 6963 6c65 2066 696c 7465  5,particle filte
+00003b70: 722c 342c 646f 6863 2c63 6f6d 6d6f 6e20  r,4,dohc,common 
+00003b80: 7261 696c 2c35 372c 3430 3030 2c38 352c  rail,57,4000,85,
+00003b90: 3132 3530 2c32 3730 2c79 6573 2c34 2c73  1250,270,yes,4,s
+00003ba0: 7461 7469 6f6e 7761 676f 6e2c 352c 6176  tationwagon,5,av
+00003bb0: 6169 6c61 626c 652c 3434 3239 352c 352c  ailable,44295,5,
+00003bc0: 3230 3135 2c6d 616e 7561 6c2c 3131 2e32  2015,manual,11.2
+00003bd0: 2c34 2e31 2c31 3039 2c43 2c33 2e37 2c32  ,4.1,109,C,3.7,2
+00003be0: 3030 2c34 2e39 2c33 2e32 332c 3230 3530  00,4.9,3.23,2050
+00003bf0: 2c31 3437 302c 3230 3930 2c37 352c 3930  ,1470,2090,75,90
+00003c00: 2c32 3939 2e31 342c 3331 362e 3639 3930  ,299.14,316.6990
+00003c10: 3239 312c 5b34 2e30 2d20 322e 3131 2d20  291,[4.0- 2.11- 
+00003c20: 312e 3338 2d20 312e 302d 2030 2e37 382d  1.38- 1.0- 0.78-
+00003c30: 2030 2e36 355d 2c31 3433 312e 3532 352c   0.65],1431.525,
+00003c40: 3135 3036 2e35 3235 2c31 3533 312e 3532  1506.525,1531.52
+00003c50: 352c 3134 3730 2c32 2e35 3837 3931 392c  5,1470,2.587919,
+00003c60: 440d 0a33 3635 3235 2c44 2c35 3138 3734  D..36525,D,51874
+00003c70: 2c79 6573 2c79 6573 2c79 6573 2c6e 6f2c  ,yes,yes,yes,no,
+00003c80: 2c6e 6f2c 3435 302c 7965 732c 7965 732c  ,no,450,yes,yes,
+00003c90: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
+00003ca0: 726f 6c2c 3838 2c31 3536 2c66 726f 6e74  rol,88,156,front
+00003cb0: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3536  ,,,,,,,,,,,1.456
+00003cc0: 2c34 2e37 3932 2c32 2e38 3137 2c31 2e38  ,4.792,2.817,1.8
+00003cd0: 3533 2c2c 3135 3938 2c72 6567 756c 6172  53,,1598,regular
+00003ce0: 2c34 2c64 6f68 632c 6d75 6c74 6970 6f69  ,4,dohc,multipoi
+00003cf0: 6e74 2069 6e6a 6563 7469 6f6e 2c37 322c  nt injection,72,
+00003d00: 3630 3030 2c38 382c 3432 3530 2c31 3536  6000,88,4250,156
+00003d10: 2c6e 6f2c 342c 7365 6461 6e2c 342c 6176  ,no,4,sedan,4,av
+00003d20: 6169 6c61 626c 652c 3239 3038 302c 352c  ailable,29080,5,
+00003d30: 3230 3134 2c61 7574 6f6d 6174 6963 2c31  2014,automatic,1
+00003d40: 312e 352c 362e 322c 3134 342c 422c 342e  1.5,6.2,144,B,4.
+00003d50: 362c 3230 332c 392c 342e 3837 2c33 3035  6,203,9,4.87,305
+00003d60: 302c 3133 3635 2c31 3934 352c 3730 2c38  0,1365,1945,70,8
+00003d70: 352e 382c 3330 332e 3832 2c33 3232 2e35  5.8,303.82,322.5
+00003d80: 3234 3237 3138 2c5b 332e 3534 2d20 312e  242718,[3.54- 1.
+00003d90: 3932 2d20 312e 3332 2d20 302e 3938 2d20  92- 1.32- 0.98- 
+00003da0: 302e 3736 2d20 302e 3635 5d2c 3133 3136  0.76- 0.65],1316
+00003db0: 2e34 2c31 3339 312e 342c 3134 3136 2e34  .4,1391.4,1416.4
+00003dc0: 2c31 3336 302c 322e 3639 3739 3638 2c44  ,1360,2.697968,D
+00003dd0: 0d0a 3437 3736 362c 442c 3638 3130 342c  ..47766,D,68104,
+00003de0: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+00003df0: 2c6e 6f2c 7965 732c 7965 732c 7965 732c  ,no,yes,yes,yes,
+00003e00: 2c66 7565 6c20 656e 6769 6e65 2c64 6965  ,fuel engine,die
+00003e10: 7365 6c2c 3838 2c33 3030 2c66 726f 6e74  sel,88,300,front
+00003e20: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3736  ,,,,,,,,,,,1.476
+00003e30: 2c34 2e38 3133 2c32 2e38 3137 2c31 2e38  ,4.813,2.817,1.8
+00003e40: 3533 2c2c 3135 3630 2c70 6172 7469 636c  53,,1560,particl
+00003e50: 6520 6669 6c74 6572 2c34 2c64 6f68 632c  e filter,4,dohc,
+00003e60: 636f 6d6d 6f6e 2072 6169 6c2c 3732 2c33  common rail,72,3
+00003e70: 3530 302c 3838 2c31 3735 302c 3330 302c  500,88,1750,300,
+00003e80: 7965 732c 322c 7374 6174 696f 6e77 6167  yes,2,stationwag
+00003e90: 6f6e 2c35 2c61 7661 696c 6162 6c65 2c33  on,5,available,3
+00003ea0: 3533 3630 2c35 2c32 3031 352c 6d61 6e75  5360,5,2015,manu
+00003eb0: 616c 2c31 312e 362c 342e 322c 3130 302c  al,11.6,4.2,100,
+00003ec0: 412c 332e 372c 3139 372c 352c 342e 3035  A,3.7,197,5,4.05
+00003ed0: 2c32 3330 302c 3134 3035 2c32 3130 302c  ,2300,1405,2100,
+00003ee0: 3830 2c38 382e 332c 3330 332e 3832 2c33  80,88.3,303.82,3
+00003ef0: 3232 2e35 3234 3237 3138 2c5b 332e 3534  22.5242718,[3.54
+00003f00: 2d20 312e 3932 2d20 312e 3332 2d20 302e  - 1.92- 1.32- 0.
+00003f10: 3938 2d20 302e 3736 2d20 302e 365d 2c31  98- 0.76- 0.6],1
+00003f20: 3335 362e 342c 3134 3331 2e34 2c31 3435  356.4,1431.4,145
+00003f30: 362e 342c 3134 3730 2c32 2e37 3335 3032  6.4,1470,2.73502
+00003f40: 382c 440d 0a36 3338 362c 442c 3737 3836  8,D..6386,D,7786
+00003f50: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
+00003f60: 2c2c 7965 732c 7965 732c 7965 732c 6e6f  ,,yes,yes,yes,no
+00003f70: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
+00003f80: 7472 6f6c 2c31 3138 2c32 3430 2c66 726f  trol,118,240,fro
+00003f90: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34  nt,,,,,,,,,,,1.4
+00003fa0: 3832 2c34 2e38 3731 2c32 2e38 352c 312e  82,4.871,2.85,1.
+00003fb0: 3835 322c 2c31 3439 382c 7265 6775 6c61  852,,1498,regula
+00003fc0: 722c 342c 646f 6863 2c64 6972 6563 7420  r,4,dohc,direct 
+00003fd0: 696e 6a65 6374 696f 6e2c 3633 2c35 3730  injection,63,570
+00003fe0: 302c 3131 382c 3136 3030 2c32 3430 2c79  0,118,1600,240,y
+00003ff0: 6573 2c34 2c68 6174 6368 6261 636b 2c35  es,4,hatchback,5
+00004000: 2c61 7661 696c 6162 6c65 2c33 3436 3935  ,available,34695
+00004010: 2c35 2c32 3031 342c 6175 746f 6d61 7469  ,5,2014,automati
+00004020: 632c 392e 312c 362e 332c 3134 362c 422c  c,9.1,6.3,146,B,
+00004030: 342e 392c 3231 342c 382e 372c 332e 3037  4.9,214,8.7,3.07
+00004040: 2c32 3230 302c 3134 3035 2c32 3139 302c  ,2200,1405,2190,
+00004050: 3735 2c37 362e 342c 3330 332e 3832 2c33  75,76.4,303.82,3
+00004060: 3232 2e35 3234 3237 3138 2c5b 342e 3538  22.5242718,[4.58
+00004070: 2d20 322e 3936 2d20 312e 3931 2d20 312e  - 2.96- 1.91- 1.
+00004080: 3435 2d20 312e 302d 2030 2e37 355d 2c31  45- 1.0- 0.75],1
+00004090: 3336 322e 3437 352c 3134 3337 2e34 3735  362.475,1437.475
+000040a0: 2c31 3436 322e 3437 352c 3134 3730 2c32  ,1462.475,1470,2
+000040b0: 2e37 3434 3636 342c 440d 0a33 3339 3538  .744664,D..33958
+000040c0: 2c44 2c34 3833 3930 2c79 6573 2c79 6573  ,D,48390,yes,yes
+000040d0: 2c79 6573 2c79 6573 2c2c 6e6f 2c79 6573  ,yes,yes,,no,yes
+000040e0: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+000040f0: 6e67 696e 652c 7065 7472 6f6c 2c31 3235  ngine,petrol,125
+00004100: 2c32 3630 2c66 726f 6e74 2c2c 2c2c 2c2c  ,260,front,,,,,,
+00004110: 2c2c 2c2c 2c31 2e35 3235 2c34 2e39 322c  ,,,,,1.525,4.92,
+00004120: 322e 3733 372c 312e 3835 382c 2c31 3539  2.737,1.858,,159
+00004130: 382c 7265 6775 6c61 722c 342c 646f 6863  8,regular,4,dohc
+00004140: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
+00004150: 6e2c 3730 2c34 3235 302c 3132 352c 3136  n,70,4250,125,16
+00004160: 3530 2c32 3630 2c79 6573 2c34 2c73 7461  50,260,yes,4,sta
+00004170: 7469 6f6e 7761 676f 6e2c 352c 6176 6169  tionwagon,5,avai
+00004180: 6c61 626c 652c 3338 3939 352c 352c 3230  lable,38995,5,20
+00004190: 3134 2c6d 616e 7561 6c2c 392e 382c 362e  14,manual,9.8,6.
+000041a0: 322c 3134 362c 422c 352e 332c 3231 352c  2,146,B,5.3,215,
+000041b0: 372e 382c 332e 3934 2c32 3730 302c 3135  7.8,3.94,2700,15
+000041c0: 3634 2c32 3231 352c 3130 302c 3831 2e35  64,2215,100,81.5
+000041d0: 2c33 3230 2e32 352c 3333 362e 3031 3934  ,320.25,336.0194
+000041e0: 3137 352c 5b34 2e32 372d 2032 2e33 352d  175,[4.27- 2.35-
+000041f0: 2031 2e34 382d 2031 2e30 372d 2030 2e38   1.48- 1.07- 0.8
+00004200: 382d 2030 2e37 345d 2c31 3531 362e 3735  8- 0.74],1516.75
+00004210: 2c31 3539 312e 3735 2c31 3631 362e 3735  ,1591.75,1616.75
+00004220: 2c31 3539 302c 322e 3833 3334 352c 440d  ,1590,2.83345,D.
+00004230: 0a33 3339 3836 2c44 2c34 3834 3138 2c79  .33986,D,48418,y
+00004240: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00004250: 6e6f 2c79 6573 2c79 6573 2c79 6573 2c2c  no,yes,yes,yes,,
+00004260: 6675 656c 2065 6e67 696e 652c 6469 6573  fuel engine,dies
+00004270: 656c 2c31 3235 2c34 3030 2c66 726f 6e74  el,125,400,front
+00004280: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35 3134  ,,,,,,,,,,,1.514
+00004290: 2c34 2e39 3133 2c32 2e37 3337 2c31 2e38  ,4.913,2.737,1.8
+000042a0: 3538 2c2c 3139 3536 2c70 6172 7469 636c  58,,1956,particl
+000042b0: 6520 6669 6c74 6572 2c34 2c64 6f68 632c  e filter,4,dohc,
+000042c0: 636f 6d6d 6f6e 2072 6169 6c2c 3730 2c33  common rail,70,3
+000042d0: 3530 302c 3132 352c 3137 3530 2c34 3030  500,125,1750,400
+000042e0: 2c79 6573 2c34 2c73 7461 7469 6f6e 7761  ,yes,4,stationwa
+000042f0: 676f 6e2c 352c 6176 6169 6c61 626c 652c  gon,5,available,
+00004300: 3433 3039 352c 352c 3230 3135 2c6d 616e  43095,5,2015,man
+00004310: 7561 6c2c 392e 392c 342e 352c 3131 392c  ual,9.9,4.5,119,
+00004320: 422c 332e 382c 3232 302c 352e 372c 332e  B,3.8,220,5.7,3.
+00004330: 3535 2c32 3035 302c 3136 3333 2c32 3330  55,2050,1633,230
+00004340: 302c 3130 302c 3930 2e34 2c33 3134 2e35  0,100,90.4,314.5
+00004350: 3935 2c33 3238 2e39 3830 3538 3235 2c5b  95,328.9805825,[
+00004360: 332e 3932 2d20 322e 3034 2d20 312e 3332  3.92- 2.04- 1.32
+00004370: 2d20 302e 3935 2d20 302e 3735 2d20 302e  - 0.95- 0.75- 0.
+00004380: 3632 5d2c 3135 3835 2e37 352c 3136 3630  62],1585.75,1660
+00004390: 2e37 352c 3136 3835 2e37 352c 3137 3030  .75,1685.75,1700
+000043a0: 2c32 2e38 3133 3031 322c 440d 0a35 3732  ,2.813012,D..572
+000043b0: 352c 442c 3730 3335 2c79 6573 2c79 6573  5,D,7035,yes,yes
+000043c0: 2c79 6573 2c79 6573 2c2c 6e6f 2c79 6573  ,yes,yes,,no,yes
+000043d0: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+000043e0: 6e67 696e 652c 7065 7472 6f6c 2c31 3231  ngine,petrol,121
+000043f0: 2c32 3130 2c66 726f 6e74 2c2c 2c2c 2c2c  ,210,front,,,,,,
+00004400: 2c2c 2c2c 2c31 2e34 382c 342e 382c 322e  ,,,,,1.48,4.8,2.
+00004410: 3735 2c31 2e38 342c 2c31 3939 382c 7265  75,1.84,,1998,re
+00004420: 6775 6c61 722c 342c 646f 6863 2c64 6972  gular,4,dohc,dir
+00004430: 6563 7420 696e 6a65 6374 696f 6e2c 3632  ect injection,62
+00004440: 2c36 3030 302c 3132 312c 3430 3030 2c32  ,6000,121,4000,2
+00004450: 3130 2c6e 6f2c 342c 7374 6174 696f 6e77  10,no,4,stationw
+00004460: 6167 6f6e 2c35 2c61 7661 696c 6162 6c65  agon,5,available
+00004470: 2c33 3539 3930 2c35 2c32 3031 352c 6175  ,35990,5,2015,au
+00004480: 746f 6d61 7469 632c 3130 2e32 2c36 2c31  tomatic,10.2,6,1
+00004490: 3339 2c42 2c35 2c32 3036 2c37 2e37 2c34  39,B,5,206,7.7,4
+000044a0: 2e33 332c 3234 3530 2c31 3331 352c 3230  .33,2450,1315,20
+000044b0: 3230 2c2c 3931 2e32 2c33 3132 2e34 3235  20,,91.2,312.425
+000044c0: 2c33 3239 2e37 3537 3238 3136 2c5b 332e  ,329.7572816,[3.
+000044d0: 3535 2d20 322e 3032 2d20 312e 3435 2d20  55- 2.02- 1.45- 
+000044e0: 312e 302d 2030 2e37 312d 2030 2e36 5d2c  1.0- 0.71- 0.6],
+000044f0: 3132 3733 2e31 352c 3133 3438 2e31 352c  1273.15,1348.15,
+00004500: 3133 3733 2e31 352c 3133 3630 2c32 2e37  1373.15,1360,2.7
+00004510: 3233 322c 440d 0a35 3731 382c 442c 3730  232,D..5718,D,70
+00004520: 3237 2c79 6573 2c79 6573 2c79 6573 2c79  27,yes,yes,yes,y
+00004530: 6573 2c2c 7965 732c 7965 732c 7965 732c  es,,yes,yes,yes,
+00004540: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00004550: 2c64 6965 7365 6c2c 3131 302c 3338 302c  ,diesel,110,380,
+00004560: 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c 2c2c  front,,,,,,,,,,,
+00004570: 312e 3438 2c34 2e38 2c32 2e37 352c 312e  1.48,4.8,2.75,1.
+00004580: 3834 2c2c 3231 3931 2c70 6172 7469 636c  84,,2191,particl
+00004590: 6520 6669 6c74 6572 2c34 2c64 6f68 632c  e filter,4,dohc,
+000045a0: 636f 6d6d 6f6e 2072 6169 6c2c 3632 2c34  common rail,62,4
+000045b0: 3530 302c 3131 302c 3230 3030 2c33 3830  500,110,2000,380
+000045c0: 2c79 6573 2c34 2c73 7461 7469 6f6e 7761  ,yes,4,stationwa
+000045d0: 676f 6e2c 352c 6176 6169 6c61 626c 652c  gon,5,available,
+000045e0: 3336 3939 302c 352c 3230 3135 2c6d 616e  36990,5,2015,man
+000045f0: 7561 6c2c 392e 322c 342e 322c 3131 302c  ual,9.2,4.2,110,
+00004600: 422c 332e 372c 3231 302c 352e 312c 322e  B,3.7,210,5.1,2.
+00004610: 3831 2c31 3935 302c 3133 3935 2c32 3039  81,1950,1395,209
+00004620: 302c 2c39 342e 332c 3331 322e 3432 352c  0,,94.3,312.425,
+00004630: 3332 392e 3735 3732 3831 362c 5b33 2e35  329.7572816,[3.5
+00004640: 342d 2031 2e38 332d 2031 2e35 372d 2031  4- 1.83- 1.57- 1
+00004650: 2e31 352d 2030 2e38 392d 2030 2e37 355d  .15- 0.89- 0.75]
+00004660: 2c31 3335 332e 3135 2c31 3432 382e 3135  ,1353.15,1428.15
+00004670: 2c31 3435 332e 3135 2c31 3437 302c 322e  ,1453.15,1470,2.
+00004680: 3732 3332 2c44 0d0a 3336 3539 312c 442c  7232,D..36591,D,
+00004690: 3531 3937 302c 7965 732c 7965 732c 7965  51970,yes,yes,ye
+000046a0: 732c 7965 732c 2c6e 6f2c 6e6f 2c79 6573  s,yes,,no,no,yes
+000046b0: 2c6e 6f2c 2c66 7565 6c20 656e 6769 6e65  ,no,,fuel engine
+000046c0: 2c70 6574 726f 6c2c 3130 382c 3139 362c  ,petrol,108,196,
+000046d0: 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c 2c2c  front,,,,,,,,,,,
+000046e0: 312e 3532 352c 342e 3731 352c 322e 372c  1.525,4.715,2.7,
+000046f0: 312e 3736 2c2c 3139 3938 2c72 6567 756c  1.76,,1998,regul
+00004700: 6172 2c34 2c64 6f68 632c 6469 7265 6374  ar,4,dohc,direct
+00004710: 2069 6e6a 6563 7469 6f6e 2c36 302c 3537   injection,60,57
+00004720: 3030 2c31 3038 2c34 3030 302c 3139 362c  00,108,4000,196,
+00004730: 6e6f 2c34 2c73 7461 7469 6f6e 7761 676f  no,4,stationwago
+00004740: 6e2c 352c 3230 3038 2c33 3139 3035 2c35  n,5,2008,31905,5
+00004750: 2c32 3030 362c 6d61 6e75 616c 2c39 2e36  ,2006,manual,9.6
+00004760: 2c38 2e31 2c31 3933 2c47 2c36 2e36 2c32  ,8.1,193,G,6.6,2
+00004770: 3130 2c31 302e 372c 332e 3638 2c32 3935  10,10.7,3.68,295
+00004780: 302c 3133 3430 2c31 3839 352c 3930 2c38  0,1340,1895,90,8
+00004790: 362c 3239 392e 3735 2c33 3133 2e39 3830  6,299.75,313.980
+000047a0: 3538 3235 2c5b 332e 3534 2d20 322e 3035  5825,[3.54- 2.05
+000047b0: 2d20 312e 3333 2d20 312e 3033 2d20 302e  - 1.33- 1.03- 0.
+000047c0: 3832 5d2c 3132 3939 2e35 2c31 3337 342e  82],1299.5,1374.
+000047d0: 352c 3133 3939 2e35 2c31 3336 302c 322e  5,1399.5,1360,2.
+000047e0: 3638 342c 440d 0a34 3335 302c 442c 3534  684,D..4350,D,54
+000047f0: 3132 2c79 6573 2c79 6573 2c79 6573 2c6e  12,yes,yes,yes,n
+00004800: 6f2c 2c6e 6f2c 6e6f 2c79 6573 2c6e 6f2c  o,,no,no,yes,no,
+00004810: 2c66 7565 6c20 656e 6769 6e65 2c64 6965  ,fuel engine,die
+00004820: 7365 6c2c 3835 2c32 3830 2c66 726f 6e74  sel,85,280,front
+00004830: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35 3235  ,,,,,,,,,,,1.525
+00004840: 2c34 2e37 2c32 2e37 2c31 2e37 362c 2c31  ,4.7,2.7,1.76,,1
+00004850: 3939 352c 6e6f 2c34 2c64 6f68 632c 636f  995,no,4,dohc,co
+00004860: 6d6d 6f6e 2072 6169 6c2c 3630 2c34 3030  mmon rail,60,400
+00004870: 302c 3835 2c32 3030 302c 3238 302c 7965  0,85,2000,280,ye
+00004880: 732c 342c 7374 6174 696f 6e77 6167 6f6e  s,4,stationwagon
+00004890: 2c35 2c32 3030 362c 3330 3230 302c 352c  ,5,2006,30200,5,
+000048a0: 3230 3033 2c6d 616e 7561 6c2c 3131 2e34  2003,manual,11.4
+000048b0: 2c36 2c31 3538 2c47 2c35 2e31 2c31 3935  ,6,158,G,5.1,195
+000048c0: 2c37 2e37 2c33 2e36 382c 3235 3530 2c31  ,7.7,3.68,2550,1
+000048d0: 3430 352c 3139 3730 2c39 302c 3934 2c32  405,1970,90,94,2
+000048e0: 3931 2e31 3435 2c33 3036 2e37 3437 3537  91.145,306.74757
+000048f0: 3238 2c5b 332e 3534 2d20 312e 3931 2d20  28,[3.54- 1.91- 
+00004900: 312e 3236 2d20 302e 3932 2d20 302e 3639  1.26- 0.92- 0.69
+00004910: 5d2c 3133 3634 2e35 2c31 3433 392e 352c  ],1364.5,1439.5,
+00004920: 3134 3634 2e35 2c31 3437 302c 322e 3638  1464.5,1470,2.68
+00004930: 342c 440d 0a33 3933 3936 2c45 2c35 3630  4,D..39396,E,560
+00004940: 3235 2c79 6573 2c79 6573 2c79 6573 2c79  25,yes,yes,yes,y
+00004950: 6573 2c2c 3834 332c 7965 732c 7965 732c  es,,843,yes,yes,
+00004960: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00004970: 2c70 6574 726f 6c2c 3232 352c 3430 302c  ,petrol,225,400,
+00004980: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
+00004990: 2c2c 2c2c 2c31 2e34 3634 2c34 2e39 3037  ,,,,,1.464,4.907
+000049a0: 2c32 2e39 3638 2c31 2e38 362c 2c32 3937  ,2.968,1.86,,297
+000049b0: 392c 7265 6775 6c61 722c 362c 646f 6863  9,regular,6,dohc
+000049c0: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
+000049d0: 6e2c 3730 2c35 3830 302c 3232 352c 3132  n,70,5800,225,12
+000049e0: 3030 2c34 3030 2c79 6573 2c34 2c73 6564  00,400,yes,4,sed
+000049f0: 616e 2c34 2c61 7661 696c 6162 6c65 2c37  an,4,available,7
+00004a00: 3032 3031 2c35 2c32 3031 332c 6175 746f  0201,5,2013,auto
+00004a10: 6d61 7469 632c 352e 362c 372e 362c 3137  matic,5.6,7.6,17
+00004a20: 382c 442c 352e 392c 3235 302c 3130 2e35  8,D,5.9,250,10.5
+00004a30: 2c33 2e30 382c 3139 3530 2c31 3734 302c  ,3.08,1950,1740,
+00004a40: 3233 3635 2c31 3030 2c38 392e 362c 3331  2365,100,89.6,31
+00004a50: 322e 3432 352c 3332 392e 3735 3732 3831  2.425,329.757281
+00004a60: 362c 5b34 2e37 312d 2033 2e31 342d 2032  6,[4.71- 3.14- 2
+00004a70: 2e31 312d 2031 2e36 372d 2031 2e32 392d  .11- 1.67- 1.29-
+00004a80: 2031 2e30 2d20 302e 3834 2d20 302e 3637   1.0- 0.84- 0.67
+00004a90: 5d2c 3136 3932 2e37 352c 3137 3637 2e37  ],1692.75,1767.7
+00004aa0: 352c 3137 3932 2e37 352c 3138 3130 2c32  5,1792.75,1810,2
+00004ab0: 2e37 3233 3034 2c45 0d0a 3430 3539 352c  .72304,E..40595,
+00004ac0: 452c 3537 3732 362c 7965 732c 7965 732c  E,57726,yes,yes,
+00004ad0: 7965 732c 7965 732c 2c38 3433 2c79 6573  yes,yes,,843,yes
+00004ae0: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+00004af0: 6e67 696e 652c 6469 6573 656c 2c31 3130  ngine,diesel,110
+00004b00: 2c33 3630 2c72 6561 722c 2c2c 2c2c 2c2c  ,360,rear,,,,,,,
+00004b10: 2c2c 2c2c 312e 3436 342c 342e 3930 372c  ,,,,1.464,4.907,
+00004b20: 322e 3936 382c 312e 3836 2c2c 3139 3935  2.968,1.86,,1995
+00004b30: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
+00004b40: 2c34 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,4,dohc,common r
+00004b50: 6169 6c2c 3730 2c34 3030 302c 3131 302c  ail,70,4000,110,
+00004b60: 3137 3530 2c33 3630 2c79 6573 2c34 2c73  1750,360,yes,4,s
+00004b70: 6564 616e 2c34 2c61 7661 696c 6162 6c65  edan,4,available
+00004b80: 2c34 3839 3835 2c35 2c32 3031 342c 6d61  ,48985,5,2014,ma
+00004b90: 6e75 616c 2c39 2e35 2c34 2e33 2c31 3134  nual,9.5,4.3,114
+00004ba0: 2c42 2c33 2e39 2c32 3138 2c35 2e31 2c33  ,B,3.9,218,5.1,3
+00004bb0: 2e32 332c 3230 3030 2c31 3539 302c 3232  .23,2000,1590,22
+00004bc0: 3235 2c31 3030 2c39 302c 3331 322e 3432  25,100,90,312.42
+00004bd0: 352c 3332 392e 3735 3732 3831 362c 5b34  5,329.7572816,[4
+00004be0: 2e31 312d 2032 2e32 352d 2031 2e34 2d20  .11- 2.25- 1.4- 
+00004bf0: 312e 302d 2030 2e38 2d20 302e 3636 5d2c  1.0- 0.8- 0.66],
+00004c00: 3135 3432 2e37 352c 3136 3137 2e37 352c  1542.75,1617.75,
+00004c10: 3136 3432 2e37 352c 3135 3930 2c32 2e37  1642.75,1590,2.7
+00004c20: 3233 3034 2c45 0d0a 3539 3039 2c45 2c37  2304,E..5909,E,7
+00004c30: 3236 322c 7965 732c 7965 732c 7965 732c  262,yes,yes,yes,
+00004c40: 7965 732c 2c6e 6f2c 7965 732c 7965 732c  yes,,no,yes,yes,
+00004c50: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00004c60: 2c70 6574 726f 6c2c 3234 352c 3434 302c  ,petrol,245,440,
+00004c70: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
+00004c80: 2c2c 2c2c 2c31 2e34 3535 2c34 2e39 3333  ,,,,,1.455,4.933
+00004c90: 2c32 2e39 3132 2c31 2e38 3734 2c2c 3239  ,2.912,1.874,,29
+00004ca0: 3935 2c72 6567 756c 6172 2c36 2c64 6f68  95,regular,6,doh
+00004cb0: 632c 6469 7265 6374 2069 6e6a 6563 7469  c,direct injecti
+00004cc0: 6f6e 2c37 352c 3535 3030 2c32 3435 2c32  on,75,5500,245,2
+00004cd0: 3930 302c 3434 302c 7965 732c 342c 7365  900,440,yes,4,se
+00004ce0: 6461 6e2c 342c 6176 6169 6c61 626c 652c  dan,4,available,
+00004cf0: 3734 3638 302c 352c 3230 3134 2c61 7574  74680,5,2014,aut
+00004d00: 6f6d 6174 6963 2c35 2e31 2c37 2e34 2c31  omatic,5.1,7.4,1
+00004d10: 3732 2c43 2c36 2c32 3530 2c39 2e38 2c34  72,C,6,250,9.8,4
+00004d20: 2e30 392c 3230 3030 2c31 3732 352c 3233  .09,2000,1725,23
+00004d30: 3630 2c31 3030 2c38 392c 3331 342e 3539  60,100,89,314.59
+00004d40: 352c 3332 382e 3938 3035 3832 352c 5b33  5,328.9805825,[3
+00004d50: 2e36 392d 2032 2e31 352d 2031 2e34 312d  .69- 2.15- 1.41-
+00004d60: 2031 2e30 332d 2030 2e37 392d 2030 2e36   1.03- 0.79- 0.6
+00004d70: 332d 2030 2e35 325d 2c31 3637 342e 3337  3- 0.52],1674.37
+00004d80: 352c 3137 3439 2e33 3735 2c31 3737 342e  5,1749.375,1774.
+00004d90: 3337 352c 3137 3030 2c32 2e37 3236 3637  375,1700,2.72667
+00004da0: 2c45 0d0a 3538 3937 2c45 2c37 3235 302c  ,E..5897,E,7250,
+00004db0: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+00004dc0: 2c6e 6f2c 7965 732c 7965 732c 7965 732c  ,no,yes,yes,yes,
+00004dd0: 2c66 7565 6c20 656e 6769 6e65 2c64 6965  ,fuel engine,die
+00004de0: 7365 6c2c 3136 302c 3530 302c 6672 6f6e  sel,160,500,fron
+00004df0: 742b 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c  t+rear,,,,,,,,,,
+00004e00: 2c31 2e34 3535 2c34 2e39 3333 2c32 2e39  ,1.455,4.933,2.9
+00004e10: 3132 2c31 2e38 3734 2c2c 3239 3637 2c70  12,1.874,,2967,p
+00004e20: 6172 7469 636c 6520 6669 6c74 6572 2c36  article filter,6
+00004e30: 2c64 6f68 632c 636f 6d6d 6f6e 2072 6169  ,dohc,common rai
+00004e40: 6c2c 3733 2c33 3235 302c 3136 302c 3132  l,73,3250,160,12
+00004e50: 3530 2c35 3030 2c79 6573 2c34 2c73 6564  50,500,yes,4,sed
+00004e60: 616e 2c34 2c61 7661 696c 6162 6c65 2c37  an,4,available,7
+00004e70: 3039 3730 2c35 2c32 3031 342c 6175 746f  0970,5,2014,auto
+00004e80: 6d61 7469 632c 362e 362c 352e 312c 3133  matic,6.6,5.1,13
+00004e90: 332c 432c 342e 362c 3234 342c 352e 392c  3,C,4.6,244,5.9,
+00004ea0: 342e 3039 2c31 3735 302c 3137 3430 2c32  4.09,1750,1740,2
+00004eb0: 3337 352c 3130 302c 3931 2e34 2c33 3230  375,100,91.4,320
+00004ec0: 2e38 362c 3333 332e 3330 3039 3730 392c  .86,333.3009709,
+00004ed0: 5b33 2e36 392d 2032 2e31 352d 2031 2e33  [3.69- 2.15- 1.3
+00004ee0: 342d 2030 2e39 372d 2030 2e37 342d 2030  4- 0.97- 0.74- 0
+00004ef0: 2e35 372d 2030 2e34 365d 2c31 3639 302e  .57- 0.46],1690.
+00004f00: 3732 352c 3137 3635 2e37 3235 2c31 3739  725,1765.725,179
+00004f10: 302e 3732 352c 3138 3130 2c32 2e37 3236  0.725,1810,2.726
+00004f20: 3637 2c45 0d0a 3539 3238 2c45 2c37 3238  67,E..5928,E,728
+00004f30: 352c 7965 732c 7965 732c 7965 732c 7965  5,yes,yes,yes,ye
+00004f40: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
+00004f50: 732c 2c66 7565 6c20 656e 6769 6e65 2c70  s,,fuel engine,p
+00004f60: 6574 726f 6c2c 3234 352c 3434 302c 6672  etrol,245,440,fr
+00004f70: 6f6e 742b 7265 6172 2c2c 2c2c 2c2c 2c2c  ont+rear,,,,,,,,
+00004f80: 2c2c 2c31 2e34 322c 342e 3937 342c 322e  ,,,1.42,4.974,2.
+00004f90: 3931 342c 312e 3931 312c 2c32 3939 352c  914,1.911,,2995,
+00004fa0: 7265 6775 6c61 722c 362c 646f 6863 2c64  regular,6,dohc,d
+00004fb0: 6972 6563 7420 696e 6a65 6374 696f 6e2c  irect injection,
+00004fc0: 3635 2c35 3330 302c 3234 352c 3239 3030  65,5300,245,2900
+00004fd0: 2c34 3430 2c79 6573 2c34 2c68 6174 6368  ,440,yes,4,hatch
+00004fe0: 6261 636b 2c35 2c61 7661 696c 6162 6c65  back,5,available
+00004ff0: 2c38 3330 3930 2c34 2c32 3031 342c 6175  ,83090,4,2014,au
+00005000: 746f 6d61 7469 632c 352e 332c 372e 362c  tomatic,5.3,7.6,
+00005010: 3137 362c 432c 362e 322c 3235 302c 3130  176,C,6.2,250,10
+00005020: 2c34 2e30 392c 3139 3530 2c31 3738 352c  ,4.09,1950,1785,
+00005030: 3234 3230 2c31 3030 2c38 392c 3331 382e  2420,100,89,318.
+00005040: 3130 352c 3333 332e 3334 3935 3134 362c  105,333.3495146,
+00005050: 5b33 2e36 392d 2032 2e31 352d 2031 2e34  [3.69- 2.15- 1.4
+00005060: 312d 2031 2e30 332d 2030 2e37 392d 2030  1- 1.03- 0.79- 0
+00005070: 2e36 332d 2030 2e35 325d 2c31 3734 312e  .63- 0.52],1741.
+00005080: 3132 352c 3138 3136 2e31 3235 2c31 3834  125,1816.125,184
+00005090: 312e 3132 352c 3138 3130 2c32 2e37 3133  1.125,1810,2.713
+000050a0: 3632 2c45 0d0a 3539 3135 2c45 2c37 3237  62,E..5915,E,727
+000050b0: 322c 7965 732c 7965 732c 7965 732c 7965  2,yes,yes,yes,ye
+000050c0: 732c 2c6e 6f2c 7965 732c 7965 732c 7965  s,,no,yes,yes,ye
+000050d0: 732c 2c66 7565 6c20 656e 6769 6e65 2c64  s,,fuel engine,d
+000050e0: 6965 7365 6c2c 3230 302c 3538 302c 6672  iesel,200,580,fr
+000050f0: 6f6e 742b 7265 6172 2c2c 2c2c 2c2c 2c2c  ont+rear,,,,,,,,
+00005100: 2c2c 2c31 2e34 322c 342e 3937 342c 322e  ,,,1.42,4.974,2.
+00005110: 3931 342c 312e 3931 312c 2c32 3936 372c  914,1.911,,2967,
+00005120: 7061 7274 6963 6c65 2066 696c 7465 722c  particle filter,
+00005130: 362c 646f 6863 2c63 6f6d 6d6f 6e20 7261  6,dohc,common ra
+00005140: 696c 2c36 352c 3335 3030 2c32 3030 2c31  il,65,3500,200,1
+00005150: 3530 302c 3538 302c 7965 732c 342c 6861  500,580,yes,4,ha
+00005160: 7463 6862 6163 6b2c 352c 6176 6169 6c61  tchback,5,availa
+00005170: 626c 652c 3738 3539 302c 342c 3230 3134  ble,78590,4,2014
+00005180: 2c61 7574 6f6d 6174 6963 2c35 2e37 2c35  ,automatic,5.7,5
+00005190: 2e32 2c31 3336 2c42 2c34 2e37 2c32 3530  .2,136,B,4.7,250
+000051a0: 2c36 2c33 2e38 382c 3136 3530 2c31 3830  ,6,3.88,1650,180
+000051b0: 352c 3234 3430 2c31 3030 2c39 312e 342c  5,2440,100,91.4,
+000051c0: 3331 382e 3130 352c 3333 332e 3334 3935  318.105,333.3495
+000051d0: 3134 362c 5b33 2e36 392d 2032 2e31 352d  146,[3.69- 2.15-
+000051e0: 2031 2e33 342d 2030 2e39 372d 2030 2e37   1.34- 0.97- 0.7
+000051f0: 342d 2030 2e35 372d 2030 2e34 365d 2c31  4- 0.57- 0.46],1
+00005200: 3736 312e 3132 352c 3138 3336 2e31 3235  761.125,1836.125
+00005210: 2c31 3836 312e 3132 352c 3138 3130 2c32  ,1861.125,1810,2
+00005220: 2e37 3133 3632 2c45 0d0a 3430 3133 302c  .71362,E..40130,
+00005230: 452c 3537 3038 342c 7965 732c 7965 732c  E,57084,yes,yes,
+00005240: 7965 732c 7965 732c 2c6e 6f2c 3131 3435  yes,yes,,no,1145
+00005250: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+00005260: 6e67 696e 652c 7065 7472 6f6c 2c31 3335  ngine,petrol,135
+00005270: 2c32 3730 2c72 6561 722c 2c2c 2c2c 2c2c  ,270,rear,,,,,,,
+00005280: 2c2c 2c2c 312e 3531 322c 342e 3839 352c  ,,,,1.512,4.895,
+00005290: 322e 3837 342c 312e 3835 342c 2c31 3739  2.874,1.854,,179
+000052a0: 362c 7265 6775 6c61 722c 342c 646f 6863  6,regular,4,dohc
+000052b0: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
+000052c0: 6e2c 3539 2c35 3235 302c 3133 352c 3138  n,59,5250,135,18
+000052d0: 3030 2c32 3730 2c79 6573 2c34 2c73 7461  00,270,yes,4,sta
+000052e0: 7469 6f6e 7761 676f 6e2c 352c 3230 3133  tionwagon,5,2013
+000052f0: 2c35 3431 3534 2c35 2c32 3031 312c 6d61  ,54154,5,2011,ma
+00005300: 6e75 616c 2c38 2e37 2c37 2e35 2c31 3735  nual,8.7,7.5,175
+00005310: 2c44 2c36 2e31 2c32 3235 2c31 302c 332e  ,D,6.1,225,10,3.
+00005320: 3037 2c32 3435 302c 3136 3335 2c32 3331  07,2450,1635,231
+00005330: 302c 3130 302c 3835 2c33 3031 2e38 3935  0,100,85,301.895
+00005340: 2c33 3136 2e36 3530 3438 3534 2c5b 342e  ,316.6504854,[4.
+00005350: 3939 2d20 322e 3832 2d20 312e 3738 2d20  99- 2.82- 1.78- 
+00005360: 312e 3235 2d20 312e 302d 2030 2e38 325d  1.25- 1.0- 0.82]
+00005370: 2c31 3539 352e 3137 352c 3136 3730 2e31  ,1595.175,1670.1
+00005380: 3735 2c31 3639 352e 3137 352c 3137 3030  75,1695.175,1700
+00005390: 2c32 2e38 3033 3234 382c 450d 0a34 3233  ,2.803248,E..423
+000053a0: 3633 2c45 2c36 3032 3434 2c79 6573 2c79  63,E,60244,yes,y
+000053b0: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c31  es,yes,yes,,no,1
+000053c0: 3134 352c 7965 732c 7965 732c 2c66 7565  145,yes,yes,,fue
+000053d0: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
+000053e0: 3137 302c 3530 302c 7265 6172 2c2c 2c2c  170,500,rear,,,,
+000053f0: 2c2c 2c2c 2c2c 2c31 2e35 3132 2c34 2e38  ,,,,,,,1.512,4.8
+00005400: 3935 2c32 2e38 3734 2c31 2e38 3534 2c2c  95,2.874,1.854,,
+00005410: 3231 3433 2c70 6172 7469 636c 6520 6669  2143,particle fi
+00005420: 6c74 6572 2c34 2c64 6f68 632c 636f 6d6d  lter,4,dohc,comm
+00005430: 6f6e 2072 6169 6c2c 3539 2c34 3230 302c  on rail,59,4200,
+00005440: 3135 302c 3136 3030 2c35 3030 2c79 6573  150,1600,500,yes
+00005450: 2c34 2c73 7461 7469 6f6e 7761 676f 6e2c  ,4,stationwagon,
+00005460: 352c 3230 3133 2c36 3238 3034 2c35 2c32  5,2013,62804,5,2
+00005470: 3031 322c 6175 746f 6d61 7469 632c 372e  012,automatic,7.
+00005480: 382c 342e 342c 3131 362c 422c 342e 342c  8,4.4,116,B,4.4,
+00005490: 3233 322c 342e 352c 322e 3635 2c31 3930  232,4.5,2.65,190
+000054a0: 302c 3138 3535 2c32 3535 352c 3130 302c  0,1855,2555,100,
+000054b0: 3939 2c33 3031 2e38 3935 2c33 3136 2e36  99,301.895,316.6
+000054c0: 3530 3438 3534 2c5b 342e 3338 2d20 322e  504854,[4.38- 2.
+000054d0: 3836 2d20 312e 3932 2d20 312e 3337 2d20  86- 1.92- 1.37- 
+000054e0: 312e 302d 2030 2e38 322d 2030 2e37 335d  1.0- 0.82- 0.73]
+000054f0: 2c31 3831 352e 3137 352c 3138 3930 2e31  ,1815.175,1890.1
+00005500: 3735 2c31 3931 352e 3137 352c 3139 3330  75,1915.175,1930
+00005510: 2c32 2e38 3033 3234 382c 450d 0a33 3437  ,2.803248,E..347
+00005520: 3630 2c45 2c34 3932 3431 2c79 6573 2c79  60,E,49241,yes,y
+00005530: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
+00005540: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00005550: 2065 6e67 696e 652c 7065 7472 6f6c 2c39   engine,petrol,9
+00005560: 322c 3230 302c 6672 6f6e 742c 2c2c 2c2c  2,200,front,,,,,
+00005570: 2c2c 2c2c 2c2c 312e 3531 2c34 2e38 3333  ,,,,,,1.51,4.833
+00005580: 2c32 2e37 3631 2c31 2e38 3137 2c2c 3133  ,2.761,1.817,,13
+00005590: 3930 2c72 6567 756c 6172 2c34 2c64 6f68  90,regular,4,doh
+000055a0: 632c 6469 7265 6374 2069 6e6a 6563 7469  c,direct injecti
+000055b0: 6f6e 2c36 302c 3530 3030 2c39 322c 3135  on,60,5000,92,15
+000055c0: 3030 2c32 3030 2c79 6573 2c34 2c73 7461  00,200,yes,4,sta
+000055d0: 7469 6f6e 7761 676f 6e2c 352c 6176 6169  tionwagon,5,avai
+000055e0: 6c61 626c 652c 3333 3033 302c 352c 3230  lable,33030,5,20
+000055f0: 3134 2c6d 616e 7561 6c2c 3130 2e36 2c36  14,manual,10.6,6
+00005600: 2e31 2c31 3432 2c42 2c35 2c32 3033 2c38  .1,142,B,5,203,8
+00005610: 2c34 2e30 362c 3236 3530 2c31 3338 392c  ,4.06,2650,1389,
+00005620: 3230 3532 2c31 3030 2c37 352e 362c 3239  2052,100,75.6,29
+00005630: 312e 3134 352c 3330 362e 3734 3735 3732  1.145,306.747572
+00005640: 382c 5b33 2e36 322d 2031 2e39 352d 2031  8,[3.62- 1.95- 1
+00005650: 2e32 382d 2030 2e39 372d 2030 2e37 382d  .28- 0.97- 0.78-
+00005660: 2030 2e36 355d 2c31 3334 382e 352c 3134   0.65],1348.5,14
+00005670: 3233 2e35 2c31 3434 382e 352c 3133 3630  23.5,1448.5,1360
+00005680: 2c32 2e37 3433 3637 2c45 0d0a 3334 3736  ,2.74367,E..3476
+00005690: 362c 452c 3439 3234 372c 7965 732c 7965  6,E,49247,yes,ye
+000056a0: 732c 7965 732c 7965 732c 2c6e 6f2c 7965  s,yes,yes,,no,ye
+000056b0: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
+000056c0: 656e 6769 6e65 2c64 6965 7365 6c2c 3737  engine,diesel,77
+000056d0: 2c32 3530 2c66 726f 6e74 2c2c 2c2c 2c2c  ,250,front,,,,,,
+000056e0: 2c2c 2c2c 2c31 2e35 312c 342e 3833 332c  ,,,,,1.51,4.833,
+000056f0: 322e 3736 312c 312e 3831 372c 2c31 3539  2.761,1.817,,159
+00005700: 382c 7061 7274 6963 6c65 2066 696c 7465  8,particle filte
+00005710: 722c 342c 646f 6863 2c63 6f6d 6d6f 6e20  r,4,dohc,common 
+00005720: 7261 696c 2c36 302c 3434 3030 2c37 372c  rail,60,4400,77,
+00005730: 3135 3030 2c32 3530 2c79 6573 2c34 2c73  1500,250,yes,4,s
+00005740: 7461 7469 6f6e 7761 676f 6e2c 352c 6176  tationwagon,5,av
+00005750: 6169 6c61 626c 652c 3333 3536 302c 352c  ailable,33560,5,
+00005760: 3230 3134 2c6d 616e 7561 6c2c 3132 2e33  2014,manual,12.3
+00005770: 2c34 2e33 2c31 3130 2c42 2c33 2e36 2c31  ,4.3,110,B,3.6,1
+00005780: 3935 2c35 2e32 2c33 2e33 392c 3230 3030  95,5.2,3.39,2000
+00005790: 2c31 3434 312c 3231 3034 2c31 3030 2c38  ,1441,2104,100,8
+000057a0: 302e 352c 3239 312e 3134 352c 3330 362e  0.5,291.145,306.
+000057b0: 3734 3735 3732 382c 5b34 2e31 312d 2032  7475728,[4.11- 2
+000057c0: 2e31 322d 2031 2e33 362d 2030 2e39 372d  .12- 1.36- 0.97-
+000057d0: 2030 2e37 332d 2030 2e35 395d 2c31 3430   0.73- 0.59],140
+000057e0: 302e 352c 3134 3735 2e35 2c31 3530 302e  0.5,1475.5,1500.
+000057f0: 352c 3134 3730 2c32 2e37 3433 3637 2c45  5,1470,2.74367,E
+00005800: 0d0a 3138 3335 2c45 2c32 3739 372c 7965  ..1835,E,2797,ye
+00005810: 732c 7965 732c 7965 732c 7965 732c 2c6e  s,yes,yes,yes,,n
+00005820: 6f2c 7965 732c 7965 732c 7965 732c 2c66  o,yes,yes,yes,,f
+00005830: 7565 6c20 656e 6769 6e65 2c64 6965 7365  uel engine,diese
+00005840: 6c2c 3135 382c 3432 302c 6672 6f6e 742c  l,158,420,front,
+00005850: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3439 332c  ,,,,,,,,,,1.493,
+00005860: 342e 3835 312c 322e 3833 352c 312e 3836  4.851,2.835,1.86
+00005870: 2c2c 3234 3030 2c70 6172 7469 636c 6520  ,,2400,particle 
+00005880: 6669 6c74 6572 2c35 2c64 6f68 632c 636f  filter,5,dohc,co
+00005890: 6d6d 6f6e 2072 6169 6c2c 3730 2c34 3030  mmon rail,70,400
+000058a0: 302c 3135 382c 3134 3030 2c34 3230 2c79  0,158,1400,420,y
+000058b0: 6573 2c34 2c73 6564 616e 2c34 2c32 3031  es,4,sedan,4,201
+000058c0: 342c 3533 3939 352c 352c 3230 3133 2c6d  4,53995,5,2013,m
+000058d0: 616e 7561 6c2c 372e 362c 342e 362c 3132  anual,7.6,4.6,12
+000058e0: 302c 422c 342c 3233 302c 352e 362c 332e  0,B,4,230,5.6,3.
+000058f0: 3737 2c31 3935 302c 3135 3335 2c32 3139  77,1950,1535,219
+00005900: 302c 3130 302c 3933 2e31 352c 3330 332e  0,100,93.15,303.
+00005910: 3635 2c33 3138 2e38 3334 3935 3135 2c5b  65,318.8349515,[
+00005920: 332e 3339 2d20 312e 3931 2d20 312e 3139  3.39- 1.91- 1.19
+00005930: 2d20 302e 3834 2d20 302e 3635 2d20 302e  - 0.84- 0.65- 0.
+00005940: 3534 5d2c 3134 3837 2e37 352c 3135 3632  54],1487.75,1562
+00005950: 2e37 352c 3135 3837 2e37 352c 3135 3930  .75,1587.75,1590
+00005960: 2c32 2e37 3736 3938 2c45 0d0a 3336 3130  ,2.77698,E..3610
+00005970: 312c 452c 3531 3237 332c 6e6f 2c79 6573  1,E,51273,no,yes
+00005980: 2c6e 6f2c 6e6f 2c2c 6e6f 2c6e 6f2c 7965  ,no,no,,no,no,ye
+00005990: 732c 6e6f 2c2c 6675 656c 2065 6e67 696e  s,no,,fuel engin
+000059a0: 652c 7065 7472 6f6c 2c31 3134 2c31 3831  e,petrol,114,181
+000059b0: 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c  ,front,,,,,,,,,,
+000059c0: 2c31 2e34 3333 2c34 2e36 3035 2c32 2e36  ,1.433,4.605,2.6
+000059d0: 362c 312e 3735 322c 2c31 3939 352c 7265  6,1.752,,1995,re
+000059e0: 6775 6c61 722c 342c 646f 6863 2c6d 756c  gular,4,dohc,mul
+000059f0: 7469 706f 696e 7420 696e 6a65 6374 696f  tipoint injectio
+00005a00: 6e2c 3635 2c36 3530 302c 3131 342c 3335  n,65,6500,114,35
+00005a10: 3030 2c31 3831 2c6e 6f2c 342c 7365 6461  00,181,no,4,seda
+00005a20: 6e2c 342c 3139 3935 2c33 3535 3939 2c35  n,4,1995,35599,5
+00005a30: 2c31 3939 342c 6175 746f 6d61 7469 632c  ,1994,automatic,
+00005a40: 3133 2e39 2c39 2e32 2c2c 2c2c 3230 342c  13.9,9.2,,,,204,
+00005a50: 2c33 2e33 352c 3236 3530 2c31 3330 302c  ,3.35,2650,1300,
+00005a60: 3138 3030 2c35 302c 3930 2c32 3731 2e35  1800,50,90,271.5
+00005a70: 3935 2c32 3839 2e33 3638 3933 322c 5b32  95,289.368932,[2
+00005a80: 2e35 382d 2031 2e34 312d 2031 2e30 2d20  .58- 1.41- 1.0- 
+00005a90: 302e 3734 5d2c 3132 3536 2e31 3235 2c31  0.74],1256.125,1
+00005aa0: 3333 312e 3132 352c 3133 3536 2e31 3235  331.125,1356.125
+00005ab0: 2c31 3336 302c 322e 3531 3036 3136 2c45  ,1360,2.510616,E
+00005ac0: 0d0a 3432 3838 362c 452c 3630 3939 332c  ..42886,E,60993,
+00005ad0: 6e6f 2c79 6573 2c6e 6f2c 6e6f 2c2c 6e6f  no,yes,no,no,,no
+00005ae0: 2c6e 6f2c 7965 732c 6e6f 2c2c 6675 656c  ,no,yes,no,,fuel
+00005af0: 2065 6e67 696e 652c 6469 6573 656c 2c38   engine,diesel,8
+00005b00: 372c 3234 352c 6672 6f6e 742c 2c2c 2c2c  7,245,front,,,,,
+00005b10: 2c2c 2c2c 2c2c 312e 3433 332c 342e 3630  ,,,,,,1.433,4.60
+00005b20: 352c 322e 3636 2c31 2e37 3532 2c2c 3235  5,2.66,1.752,,25
+00005b30: 3030 2c6e 6f2c 342c 6f68 632c 696e 6469  00,no,4,ohc,indi
+00005b40: 7265 6374 2069 6e6a 6563 7469 6f6e 2c36  rect injection,6
+00005b50: 352c 3431 3030 2c38 372c 3234 3030 2c32  5,4100,87,2400,2
+00005b60: 3435 2c79 6573 2c32 2c73 6564 616e 2c34  45,yes,2,sedan,4
+00005b70: 2c31 3939 352c 3338 3638 352c 352c 3139  ,1995,38685,5,19
+00005b80: 3932 2c6d 616e 7561 6c2c 3131 2e35 2c37  92,manual,11.5,7
+00005b90: 2e32 2c2c 2c2c 3139 322c 2c33 2e35 362c  .2,,,,192,,3.56,
+00005ba0: 3236 3530 2c31 3332 362c 3138 3235 2c35  2650,1326,1825,5
+00005bb0: 302c 3932 2c32 3831 2e37 362c 3239 382e  0,92,281.76,298.
+00005bc0: 3534 3336 3839 332c 5b33 2e37 352d 2032  5436893,[3.75- 2
+00005bd0: 2e31 382d 2031 2e33 382d 2030 2e39 382d  .18- 1.38- 0.98-
+00005be0: 2030 2e37 325d 2c31 3238 322e 3132 352c   0.72],1282.125,
+00005bf0: 3133 3537 2e31 3235 2c31 3338 322e 3132  1357.125,1382.12
+00005c00: 352c 3133 3630 2c32 2e35 3130 3631 362c  5,1360,2.510616,
+00005c10: 450d 0a31 3433 312c 452c 3137 3830 2c79  E..1431,E,1780,y
+00005c20: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00005c30: 7965 732c 6e6f 2c79 6573 2c6e 6f2c 2c66  yes,no,yes,no,,f
+00005c40: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
+00005c50: 6c2c 3138 332c 3331 302c 7265 6172 2c2c  l,183,310,rear,,
+00005c60: 2c2c 2c2c 2c2c 2c2c 2c31 2e34 332c 342e  ,,,,,,,,,1.43,4.
+00005c70: 3832 352c 322e 3835 2c31 2e38 3135 2c2c  825,2.85,1.815,,
+00005c80: 3239 3935 2c72 6567 756c 6172 2c36 2c64  2995,regular,6,d
+00005c90: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
+00005ca0: 7469 6f6e 2c37 312c 3632 3030 2c31 3833  tion,71,6200,183
+00005cb0: 2c33 3530 302c 3331 302c 6e6f 2c34 2c73  ,3500,310,no,4,s
+00005cc0: 6564 616e 2c34 2c32 3031 302c 3635 3430  edan,4,2010,6540
+00005cd0: 352c 352c 3230 3038 2c61 7574 6f6d 6174  5,5,2008,automat
+00005ce0: 6963 2c37 2e32 2c39 2e35 2c32 3234 2c47  ic,7.2,9.5,224,G
+00005cf0: 2c37 2c32 3430 2c31 342c 332e 3733 2c2c  ,7,240,14,3.73,,
+00005d00: 3135 3935 2c32 3132 352c 3735 2c38 332c  1595,2125,75,83,
+00005d10: 3330 332e 3635 2c33 3138 2e38 3334 3935  303.65,318.83495
+00005d20: 3135 2c5b 332e 3534 2d20 322e 3036 2d20  15,[3.54- 2.06- 
+00005d30: 312e 342d 2031 2e30 2d20 302e 3731 2d20  1.4- 1.0- 0.71- 
+00005d40: 302e 3538 5d2c 3135 3437 2e30 3735 2c31  0.58],1547.075,1
+00005d50: 3632 322e 3037 352c 3136 3437 2e30 3735  622.075,1647.075
+00005d60: 2c31 3539 302c 322e 3539 3534 352c 450d  ,1590,2.59545,E.
+00005d70: 0a34 3635 3437 2c46 2c36 3633 3539 2c79  .46547,F,66359,y
+00005d80: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00005d90: 7965 732c 7965 732c 7965 732c 6e6f 2c2c  yes,yes,yes,no,,
+00005da0: 6675 656c 2065 6e67 696e 652c 7065 7472  fuel engine,petr
+00005db0: 6f6c 2c33 3830 2c38 3330 2c72 6561 722c  ol,380,830,rear,
+00005dc0: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3438 352c  ,,,,,,,,,,1.485,
+00005dd0: 352e 3232 362c 332e 3136 352c 312e 3837  5.226,3.165,1.87
+00005de0: 312c 2c35 3531 332c 7265 6775 6c61 722c  1,,5513,regular,
+00005df0: 3132 2c6f 6863 2c6d 756c 7469 706f 696e  12,ohc,multipoin
+00005e00: 7420 696e 6a65 6374 696f 6e2c 3930 2c35  t injection,90,5
+00005e10: 3030 302c 3338 302c 3138 3030 2c38 3330  000,380,1800,830
+00005e20: 2c79 6573 2c33 2c73 6564 616e 2c34 2c32  ,yes,3,sedan,4,2
+00005e30: 3031 332c 3233 3934 3530 2c35 2c32 3031  013,239450,5,201
+00005e40: 312c 6175 746f 6d61 7469 632c 342e 362c  1,automatic,4.6,
+00005e50: 3134 2e31 2c33 3239 2c47 2c39 2e37 2c32  14.1,329,G,9.7,2
+00005e60: 3530 2c32 312e 352c 322e 3635 2c32 3035  50,21.5,2.65,205
+00005e70: 302c 3231 3130 2c32 3639 302c 3130 302c  0,2110,2690,100,
+00005e80: 3837 2c33 3138 2e31 3035 2c33 3333 2e33  87,318.105,333.3
+00005e90: 3439 3531 3436 2c5b 332e 362d 2032 2e31  495146,[3.6- 2.1
+00005ea0: 392d 2031 2e34 2d20 312e 302d 2030 2e38  9- 1.4- 1.0- 0.8
+00005eb0: 335d 2c32 3034 392e 3235 2c32 3132 342e  3],2049.25,2124.
+00005ec0: 3235 2c32 3134 392e 3235 2c32 3135 302c  25,2149.25,2150,
+00005ed0: 322e 3737 3834 3335 2c46 0d0a 3434 3739  2.778435,F..4479
+00005ee0: 392c 462c 3633 3736 322c 7965 732c 7965  9,F,63762,yes,ye
+00005ef0: 732c 7965 732c 7965 732c 2c6e 6f2c 3131  s,yes,yes,,no,11
+00005f00: 3435 2c79 6573 2c79 6573 2c2c 6675 656c  45,yes,yes,,fuel
+00005f10: 2065 6e67 696e 652c 6469 6573 656c 2c31   engine,diesel,1
+00005f20: 3530 2c35 3030 2c72 6561 722c 2c2c 2c2c  50,500,rear,,,,,
+00005f30: 2c2c 2c2c 2c2c 312e 3438 352c 352e 3039  ,,,,,,1.485,5.09
+00005f40: 362c 332e 3033 352c 312e 3837 312c 2c32  6,3.035,1.871,,2
+00005f50: 3134 332c 7061 7274 6963 6c65 2066 696c  143,particle fil
+00005f60: 7465 722c 342c 646f 6863 2c63 6f6d 6d6f  ter,4,dohc,commo
+00005f70: 6e20 7261 696c 2c38 332c 3432 3030 2c31  n rail,83,4200,1
+00005f80: 3530 2c31 3630 302c 3530 302c 7965 732c  50,1600,500,yes,
+00005f90: 342c 7365 6461 6e2c 342c 3230 3133 2c38  4,sedan,4,2013,8
+00005fa0: 3739 3530 2c35 2c32 3031 312c 6175 746f  7950,5,2011,auto
+00005fb0: 6d61 7469 632c 382e 322c 352e 372c 3134  matic,8.2,5.7,14
+00005fc0: 392c 432c 352c 3234 302c 372c 322e 3832  9,C,5,240,7,2.82
+00005fd0: 2c31 3930 302c 3138 3730 2c32 3536 352c  ,1900,1870,2565,
+00005fe0: 3130 302c 3939 2c33 3136 2e37 3135 2c33  100,99,316.715,3
+00005ff0: 3335 2e30 3937 3038 3734 2c5b 342e 3338  35.0970874,[4.38
+00006000: 2d20 322e 3836 2d20 312e 3932 2d20 312e  - 2.86- 1.92- 1.
+00006010: 3337 2d20 312e 302d 2030 2e38 322d 2030  37- 1.0- 0.82- 0
+00006020: 2e37 335d 2c31 3831 332e 3937 352c 3138  .73],1813.975,18
+00006030: 3838 2e39 3735 2c31 3931 332e 3937 352c  88.975,1913.975,
+00006040: 3139 3330 2c32 2e37 3738 3433 352c 460d  1930,2.778435,F.
+00006050: 0a34 3130 3435 2c46 2c35 3833 3632 2c79  .41045,F,58362,y
+00006060: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00006070: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+00006080: 2c66 7565 6c20 656e 6769 6e65 2c70 6574  ,fuel engine,pet
+00006090: 726f 6c2c 3336 382c 3632 352c 6672 6f6e  rol,368,625,fron
+000060a0: 742b 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c  t+rear,,,,,,,,,,
+000060b0: 2c31 2e34 3731 2c35 2e32 3635 2c33 2e31  ,1.471,5.265,3.1
+000060c0: 3232 2c31 2e39 3439 2c2c 3632 3939 2c72  22,1.949,,6299,r
+000060d0: 6567 756c 6172 2c31 322c 646f 6863 2c64  egular,12,dohc,d
+000060e0: 6972 6563 7420 696e 6a65 6374 696f 6e2c  irect injection,
+000060f0: 3832 2c36 3230 302c 3336 382c 3437 3530  82,6200,368,4750
+00006100: 2c36 3235 2c6e 6f2c 342c 7365 6461 6e2c  ,625,no,4,sedan,
+00006110: 342c 6176 6169 6c61 626c 652c 3232 3536  4,available,2256
+00006120: 3530 2c35 2c32 3031 342c 6175 746f 6d61  50,5,2014,automa
+00006130: 7469 632c 342e 362c 3131 2e33 2c32 3634  tic,4.6,11.3,264
+00006140: 2c47 2c38 2e37 2c32 3530 2c31 352e 372c  ,G,8.7,250,15.7,
+00006150: 332e 3038 2c31 3835 302c 3230 3530 2c32  3.08,1850,2050,2
+00006160: 3637 352c 3130 302c 3930 2e34 2c33 3330  675,100,90.4,330
+00006170: 2e38 3035 2c33 3435 2e36 3739 3631 3137  .805,345.6796117
+00006180: 2c5b 342e 3731 2d20 332e 3134 2d20 322e  ,[4.71- 3.14- 2.
+00006190: 3131 2d20 312e 3637 2d20 312e 3239 2d20  11- 1.67- 1.29- 
+000061a0: 312e 302d 2030 2e38 342d 2030 2e36 375d  1.0- 0.84- 0.67]
+000061b0: 2c31 3939 342e 3635 2c32 3036 392e 3635  ,1994.65,2069.65
+000061c0: 2c32 3039 342e 3635 2c32 3034 302c 322e  ,2094.65,2040,2.
+000061d0: 3836 3639 3739 2c46 0d0a 3339 3832 302c  866979,F..39820,
+000061e0: 462c 3536 3634 312c 7965 732c 7965 732c  F,56641,yes,yes,
+000061f0: 7965 732c 7965 732c 2c31 3437 312c 7965  yes,yes,,1471,ye
+00006200: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
+00006210: 656e 6769 6e65 2c64 6965 7365 6c2c 3139  engine,diesel,19
+00006220: 302c 3538 302c 6672 6f6e 742b 7265 6172  0,580,front+rear
+00006230: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e34 362c  ,,,,,,,,,,,1.46,
+00006240: 352e 3236 352c 332e 3132 322c 312e 3934  5.265,3.122,1.94
+00006250: 392c 2c32 3936 372c 7061 7274 6963 6c65  9,,2967,particle
+00006260: 2066 696c 7465 722c 362c 646f 6863 2c63   filter,6,dohc,c
+00006270: 6f6d 6d6f 6e20 7261 696c 2c38 322c 3430  ommon rail,82,40
+00006280: 3030 2c31 3930 2c31 3735 302c 3538 302c  00,190,1750,580,
+00006290: 7965 732c 342c 7365 6461 6e2c 342c 6176  yes,4,sedan,4,av
+000062a0: 6169 6c61 626c 652c 3130 3131 3330 2c35  ailable,101130,5
+000062b0: 2c32 3031 332c 6175 746f 6d61 7469 632c  ,2013,automatic,
+000062c0: 362e 312c 362c 3135 382c 422c 352e 322c  6.1,6,158,B,5.2,
+000062d0: 3235 302c 372e 352c 322e 3338 2c31 3430  250,7.5,2.38,140
+000062e0: 302c 3139 3130 2c32 3538 352c 3130 302c  0,1910,2585,100,
+000062f0: 3931 2e34 2c33 3239 2e34 3135 2c33 3437  91.4,329.415,347
+00006300: 2e34 3237 3138 3435 2c5b 342e 3731 2d20  .4271845,[4.71- 
+00006310: 332e 3134 2d20 322e 3131 2d20 312e 3637  3.14- 2.11- 1.67
+00006320: 2d20 312e 3239 2d20 312e 302d 2030 2e38  - 1.29- 1.0- 0.8
+00006330: 342d 2030 2e36 375d 2c31 3835 342e 3635  4- 0.67],1854.65
+00006340: 2c31 3932 392e 3635 2c31 3935 342e 3635  ,1929.65,1954.65
+00006350: 2c31 3933 302c 322e 3834 3535 342c 460d  ,1930,2.84554,F.
+00006360: 0a33 3431 3833 2c46 2c34 3836 3330 2c79  .34183,F,48630,y
+00006370: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00006380: 6e6f 2c79 6573 2c79 6573 2c79 6573 2c2c  no,yes,yes,yes,,
+00006390: 6675 656c 2065 6e67 696e 652c 7065 7472  fuel engine,petr
+000063a0: 6f6c 2c32 3238 2c34 3030 2c66 726f 6e74  ol,228,400,front
+000063b0: 2b72 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c  +rear,,,,,,,,,,,
+000063c0: 312e 3431 382c 352e 3031 352c 322e 3932  1.418,5.015,2.92
+000063d0: 2c31 2e39 3331 2c2c 3336 3035 2c72 6567  ,1.931,,3605,reg
+000063e0: 756c 6172 2c36 2c64 6f68 632c 6469 7265  ular,6,dohc,dire
+000063f0: 6374 2069 6e6a 6563 7469 6f6e 2c31 3030  ct injection,100
+00006400: 2c36 3230 302c 3232 382c 3337 3530 2c34  ,6200,228,3750,4
+00006410: 3030 2c6e 6f2c 342c 6861 7463 6862 6163  00,no,4,hatchbac
+00006420: 6b2c 352c 6176 6169 6c61 626c 652c 3131  k,5,available,11
+00006430: 3335 3030 2c34 2c32 3031 332c 6175 746f  3500,4,2013,auto
+00006440: 6d61 7469 632c 362e 312c 382e 372c 3230  matic,6.1,8.7,20
+00006450: 332c 442c 372e 312c 3235 372c 3131 2e34  3,D,7.1,257,11.4
+00006460: 2c33 2e39 2c32 3130 302c 3138 3230 2c32  ,3.9,2100,1820,2
+00006470: 3432 302c 3735 2c38 332c 3332 342e 3135  420,75,83,324.15
+00006480: 2c33 3430 2e38 3733 3738 3634 2c5b 352e  ,340.8737864,[5.
+00006490: 3937 2d20 332e 3331 2d20 322e 3031 2d20  97- 3.31- 2.01- 
+000064a0: 312e 3337 2d20 312e 302d 2030 2e38 312d  1.37- 1.0- 0.81-
+000064b0: 2030 2e35 395d 2c31 3735 322e 352c 3138   0.59],1752.5,18
+000064c0: 3237 2e35 2c31 3835 322e 352c 3138 3130  27.5,1852.5,1810
+000064d0: 2c32 2e37 3338 3135 382c 460d 0a33 3431  ,2.738158,F..341
+000064e0: 3836 2c46 2c34 3836 3334 2c79 6573 2c79  86,F,48634,yes,y
+000064f0: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
+00006500: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00006510: 2065 6e67 696e 652c 6469 6573 656c 2c32   engine,diesel,2
+00006520: 3231 2c36 3530 2c72 6561 722c 2c2c 2c2c  21,650,rear,,,,,
+00006530: 2c2c 2c2c 2c2c 312e 3431 382c 352e 3031  ,,,,,,1.418,5.01
+00006540: 352c 322e 3932 2c31 2e39 3331 2c2c 3239  5,2.92,1.931,,29
+00006550: 3637 2c70 6172 7469 636c 6520 6669 6c74  67,particle filt
+00006560: 6572 2c36 2c64 6f68 632c 636f 6d6d 6f6e  er,6,dohc,common
+00006570: 2072 6169 6c2c 3830 2c34 3030 302c 3232   rail,80,4000,22
+00006580: 312c 3137 3530 2c36 3530 2c79 6573 2c34  1,1750,650,yes,4
+00006590: 2c68 6174 6368 6261 636b 2c35 2c61 7661  ,hatchback,5,ava
+000065a0: 696c 6162 6c65 2c31 3036 3430 302c 342c  ilable,106400,4,
+000065b0: 3230 3134 2c61 7574 6f6d 6174 6963 2c36  2014,automatic,6
+000065c0: 2c36 2e34 2c31 3639 2c44 2c35 2e36 2c32  ,6.4,169,D,5.6,2
+000065d0: 3539 2c37 2e37 2c32 2e36 392c 3137 3030  59,7.7,2.69,1700
+000065e0: 2c31 3930 302c 3235 3030 2c37 352c 3931  ,1900,2500,75,91
+000065f0: 2e34 2c33 3234 2e31 352c 3334 302e 3837  .4,324.15,340.87
+00006600: 3337 3836 342c 5b34 2e39 322d 2032 2e38  37864,[4.92- 2.8
+00006610: 312d 2031 2e38 342d 2031 2e34 332d 2031  1- 1.84- 1.43- 1
+00006620: 2e32 312d 2031 2e30 2d20 302e 3833 2d20  .21- 1.0- 0.83- 
+00006630: 302e 3639 5d2c 3138 3436 2c31 3932 312c  0.69],1846,1921,
+00006640: 3139 3436 2c31 3933 302c 322e 3733 3831  1946,1930,2.7381
+00006650: 3538 2c46 0d0a 3230 3631 322c 462c 3238  58,F..20612,F,28
+00006660: 3032 312c 7965 732c 7965 732c 7965 732c  021,yes,yes,yes,
+00006670: 7965 732c 2c31 3939 302c 3133 3235 2c79  yes,,1990,1325,y
+00006680: 6573 2c6e 6f2c 2c66 7565 6c20 656e 6769  es,no,,fuel engi
+00006690: 6e65 2c70 6574 726f 6c2c 3234 362c 3433  ne,petrol,246,43
+000066a0: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
+000066b0: 2c2c 2c2c 2c2c 2c31 2e34 352c 352e 3035  ,,,,,,,1.45,5.05
+000066c0: 392c 322e 3838 312c 312e 3930 332c 2c34  9,2.881,1.903,,4
+000066d0: 3137 322c 7265 6775 6c61 722c 382c 646f  172,regular,8,do
+000066e0: 6863 2c6d 756c 7469 706f 696e 7420 696e  hc,multipoint in
+000066f0: 6a65 6374 696f 6e2c 3930 2c36 3530 302c  jection,90,6500,
+00006700: 3234 362c 3335 3030 2c34 3330 2c6e 6f2c  246,3500,430,no,
+00006710: 342c 7365 6461 6e2c 342c 6176 6169 6c61  4,sedan,4,availa
+00006720: 626c 652c 3134 3835 3930 2c35 2c32 3031  ble,148590,5,201
+00006730: 302c 6175 746f 6d61 7469 632c 362e 392c  0,automatic,6.9,
+00006740: 3132 2e35 2c32 3930 2c47 2c39 2e32 2c32  12.5,290,G,9.2,2
+00006750: 3530 2c31 382e 322c 332e 3331 2c32 3130  50,18.2,3.31,210
+00006760: 302c 3230 3832 2c32 3730 302c 3130 302c  0,2082,2700,100,
+00006770: 3933 2c33 3136 2e37 3135 2c33 3335 2e30  93,316.715,335.0
+00006780: 3937 3038 3734 2c5b 342e 3137 2d20 322e  970874,[4.17- 2.
+00006790: 3334 2d20 312e 3532 2d20 312e 3134 2d20  34- 1.52- 1.14- 
+000067a0: 302e 3837 2d20 302e 3639 5d2c 3230 3231  0.87- 0.69],2021
+000067b0: 2e32 352c 3230 3936 2e32 352c 3231 3231  .25,2096.25,2121
+000067c0: 2e32 352c 3230 3430 2c32 2e37 3539 3335  .25,2040,2.75935
+000067d0: 2c46 0d0a 3230 3630 352c 462c 3238 3031  ,F..20605,F,2801
+000067e0: 342c 7965 732c 7965 732c 7965 732c 7965  4,yes,yes,yes,ye
+000067f0: 732c 2c31 3939 302c 7965 732c 7965 732c  s,,1990,yes,yes,
+00006800: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
+00006810: 6469 6573 656c 2c31 3830 2c35 3030 2c66  diesel,180,500,f
+00006820: 726f 6e74 2b72 6561 722c 2c2c 2c2c 2c2c  ront+rear,,,,,,,
+00006830: 2c2c 2c2c 312e 3435 2c35 2e30 3539 2c32  ,,,,1.45,5.059,2
+00006840: 2e38 3831 2c31 2e39 3033 2c2c 3239 3637  .881,1.903,,2967
+00006850: 2c70 6172 7469 636c 6520 6669 6c74 6572  ,particle filter
+00006860: 2c36 2c64 6f68 632c 636f 6d6d 6f6e 2072  ,6,dohc,common r
+00006870: 6169 6c2c 3930 2c34 3030 302c 3138 302c  ail,90,4000,180,
+00006880: 3135 3030 2c35 3030 2c79 6573 2c34 2c73  1500,500,yes,4,s
+00006890: 6564 616e 2c34 2c61 7661 696c 6162 6c65  edan,4,available
+000068a0: 2c31 3038 3839 302c 352c 3230 3133 2c61  ,108890,5,2013,a
+000068b0: 7574 6f6d 6174 6963 2c38 2e33 2c38 2e35  utomatic,8.3,8.5
+000068c0: 2c32 3234 2c47 2c36 2e37 2c32 3338 2c31  ,224,G,6.7,238,1
+000068d0: 312e 362c 332e 3333 2c32 3130 302c 3231  1.6,3.33,2100,21
+000068e0: 3333 2c32 3736 302c 3130 302c 3931 2e34  33,2760,100,91.4
+000068f0: 2c33 3133 2e31 382c 3333 342e 3137 3437  ,313.18,334.1747
+00006900: 3537 332c 5b34 2e31 372d 2032 2e33 342d  573,[4.17- 2.34-
+00006910: 2031 2e35 322d 2031 2e31 342d 2030 2e38   1.52- 1.14- 0.8
+00006920: 372d 2030 2e36 395d 2c32 3037 322e 3235  7- 0.69],2072.25
+00006930: 2c32 3134 372e 3235 2c32 3137 322e 3235  ,2147.25,2172.25
+00006940: 2c32 3135 302c 322e 3735 3933 352c 460d  ,2150,2.75935,F.
+00006950: 0a31 3332 342c 462c 3135 3136 2c79 6573  .1324,F,1516,yes
+00006960: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
+00006970: 2c79 6573 2c79 6573 2c6e 6f2c 2c66 7565  ,yes,yes,no,,fue
+00006980: 6c20 656e 6769 6e65 2c70 6574 726f 6c2c  l engine,petrol,
+00006990: 3232 342c 3432 302c 7265 6172 2c2c 2c2c  224,420,rear,,,,
+000069a0: 2c2c 2c2c 2c2c 2c31 2e34 3535 2c35 2e32  ,,,,,,,1.455,5.2
+000069b0: 3135 2c33 2e31 3539 2c31 2e38 362c 2c34  15,3.159,1.86,,4
+000069c0: 3139 362c 7265 6775 6c61 722c 382c 646f  196,regular,8,do
+000069d0: 6863 2c6d 756c 7469 706f 696e 7420 696e  hc,multipoint in
+000069e0: 6a65 6374 696f 6e2c 3835 2c36 3030 302c  jection,85,6000,
+000069f0: 3232 342c 3431 3030 2c34 3230 2c6e 6f2c  224,4100,420,no,
+00006a00: 342c 7365 6461 6e2c 342c 3230 3039 2c31  4,sedan,4,2009,1
+00006a10: 3231 3039 302c 352c 3230 3039 2c61 7574  21090,5,2009,aut
+00006a20: 6f6d 6174 6963 2c36 2e36 2c31 312e 342c  omatic,6.6,11.4,
+00006a30: 3236 392c 472c 382e 342c 3235 302c 3136  269,G,8.4,250,16
+00006a40: 2e37 2c32 2e38 372c 3138 3530 2c31 3631  .7,2.87,1850,161
+00006a50: 352c 3232 3436 2c37 352c 3930 2e33 2c33  5,2246,75,90.3,3
+00006a60: 3230 2e38 362c 3333 332e 3330 3039 3730  20.86,333.300970
+00006a70: 392c 5b34 2e31 372d 2032 2e33 342d 2031  9,[4.17- 2.34- 1
+00006a80: 2e35 322d 2031 2e31 342d 2030 2e38 372d  .52- 1.14- 0.87-
+00006a90: 2030 2e36 395d 2c31 3535 372e 3632 352c   0.69],1557.625,
+00006aa0: 3136 3332 2e36 3235 2c31 3635 372e 3632  1632.625,1657.62
+00006ab0: 352c 3135 3930 2c32 2e37 3036 332c 460d  5,1590,2.7063,F.
+00006ac0: 0a39 3838 322c 462c 3132 3337 352c 7965  .9882,F,12375,ye
+00006ad0: 732c 7965 732c 7965 732c 7965 732c 2c79  s,yes,yes,yes,,y
+00006ae0: 6573 2c79 6573 2c79 6573 2c6e 6f2c 2c66  es,yes,yes,no,,f
+00006af0: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
+00006b00: 6c2c 3330 312c 3535 302c 7265 6172 2c2c  l,301,550,rear,,
+00006b10: 2c2c 2c2c 2c2c 2c2c 2c31 2e34 3831 2c35  ,,,,,,,,,1.481,5
+00006b20: 2e32 3632 2c33 2e31 3731 2c31 2e39 3438  .262,3.171,1.948
+00006b30: 2c2c 3239 3739 2c72 6567 756c 6172 2c36  ,,2979,regular,6
+00006b40: 2c64 6f68 632c 6469 7265 6374 2069 6e6a  ,dohc,direct inj
+00006b50: 6563 7469 6f6e 2c38 302c 3535 3030 2c33  ection,80,5500,3
+00006b60: 3031 2c31 3735 302c 3535 302c 7965 732c  01,1750,550,yes,
+00006b70: 342c 7365 6461 6e2c 342c 6176 6169 6c61  4,sedan,4,availa
+00006b80: 626c 652c 3133 3938 3231 2c35 2c32 3031  ble,139821,5,201
+00006b90: 342c 6175 746f 6d61 7469 632c 352e 312c  4,automatic,5.1,
+00006ba0: 3130 2e35 2c32 3434 2c46 2c37 2e37 2c32  10.5,244,F,7.7,2
+00006bb0: 3835 2c31 352e 332c 332e 3733 2c2c 3139  85,15.3,3.73,,19
+00006bc0: 3230 2c32 3534 302c 2c38 342e 352c 3332  20,2540,,84.5,32
+00006bd0: 372e 3239 352c 3334 312e 3331 3036 3739  7.295,341.310679
+00006be0: 362c 5b33 2e32 392d 2032 2e31 362d 2031  6,[3.29- 2.16- 1
+00006bf0: 2e36 312d 2031 2e32 372d 2031 2e30 332d  .61- 1.27- 1.03-
+00006c00: 2030 2e38 355d 2c31 3836 362c 3139 3431   0.85],1866,1941
+00006c10: 2c31 3936 362c 3139 3330 2c32 2e38 3834  ,1966,1930,2.884
+00006c20: 3938 382c 460d 0a34 3935 372c 462c 3631  988,F..4957,F,61
+00006c30: 3132 2c79 6573 2c79 6573 2c79 6573 2c79  12,yes,yes,yes,y
+00006c40: 6573 2c2c 6e6f 2c79 6573 2c79 6573 2c6e  es,,no,yes,yes,n
+00006c50: 6f2c 2c66 7565 6c20 656e 6769 6e65 2c70  o,,fuel engine,p
+00006c60: 6574 726f 6c2c 3337 332c 3939 392c 7265  etrol,373,999,re
+00006c70: 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e35  ar,,,,,,,,,,,1.5
+00006c80: 3135 2c35 2e34 2c33 2e31 3136 2c31 2e39  15,5.4,3.116,1.9
+00006c90: 2c2c 3637 3631 2c72 6567 756c 6172 2c38  ,,6761,regular,8
+00006ca0: 2c6f 6876 2c6d 756c 7469 706f 696e 7420  ,ohv,multipoint 
+00006cb0: 696e 6a65 6374 696f 6e2c 3936 2c34 3230  injection,96,420
+00006cc0: 302c 3337 332c 3332 3030 2c39 3939 2c79  0,373,3200,999,y
+00006cd0: 6573 2c32 2c73 6564 616e 2c34 2c32 3031  es,2,sedan,4,201
+00006ce0: 302c 2c35 2c32 3030 372c 6175 746f 6d61  0,,5,2007,automa
+00006cf0: 7469 632c 352e 352c 3139 2e35 2c34 3635  tic,5.5,19.5,465
+00006d00: 2c47 2c31 342e 312c 3238 382c 3238 2e38  ,G,14.1,288,28.8
+00006d10: 2c32 2e36 392c 2c32 3538 352c 3330 3635  ,2.69,,2585,3065
+00006d20: 2c2c 3939 2e31 2c33 3330 2e38 3035 2c33  ,,99.1,330.805,3
+00006d30: 3435 2e36 3739 3631 3137 2c5b 322e 3438  45.6796117,[2.48
+00006d40: 2d20 312e 3438 2d20 312e 302d 2030 2e37  - 1.48- 1.0- 0.7
+00006d50: 355d 2c32 3532 302e 322c 3235 3935 2e32  5],2520.2,2595.2
+00006d60: 2c32 3632 302e 322c 3232 3730 2c32 2e38  ,2620.2,2270,2.8
+00006d70: 3738 352c 460d 0a35 3539 352c 532c 3638  785,F..5595,S,68
+00006d80: 3639 2c79 6573 2c79 6573 2c79 6573 2c79  69,yes,yes,yes,y
+00006d90: 6573 2c2c 3936 362c 7965 732c 7965 732c  es,,966,yes,yes,
+00006da0: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00006db0: 2c70 6574 726f 6c2c 3233 352c 3435 302c  ,petrol,235,450,
+00006dc0: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
+00006dd0: 2c2c 2c2c 2c31 2e33 3635 2c34 2e38 3934  ,,,,,1.365,4.894
+00006de0: 2c32 2e38 3535 2c31 2e38 3934 2c2c 3239  ,2.855,1.894,,29
+00006df0: 3739 2c72 6567 756c 6172 2c36 2c64 6f68  79,regular,6,doh
+00006e00: 632c 6469 7265 6374 2069 6e6a 6563 7469  c,direct injecti
+00006e10: 6f6e 2c37 302c 3538 3030 2c32 3335 2c31  on,70,5800,235,1
+00006e20: 3330 302c 3435 302c 7965 732c 342c 6361  300,450,yes,4,ca
+00006e30: 6272 696f 6c65 742c 322c 6176 6169 6c61  briolet,2,availa
+00006e40: 626c 652c 3132 3038 3935 2c34 2c32 3031  ble,120895,4,201
+00006e50: 352c 6175 746f 6d61 7469 632c 352e 342c  5,automatic,5.4,
+00006e60: 382e 322c 3139 312c 442c 362e 332c 3235  8.2,191,D,6.3,25
+00006e70: 302c 3131 2e34 2c33 2e32 332c 3230 3530  0,11.4,3.23,2050
+00006e80: 2c31 3836 352c 3233 3930 2c30 2c38 392e  ,1865,2390,0,89.
+00006e90: 362c 3331 342e 3539 352c 3332 382e 3938  6,314.595,328.98
+00006ea0: 3035 3832 352c 5b34 2e37 312d 2033 2e31  05825,[4.71- 3.1
+00006eb0: 342d 2032 2e31 312d 2031 2e36 372d 2031  4- 2.11- 1.67- 1
+00006ec0: 2e32 392d 2031 2e30 2d20 302e 3834 2d20  .29- 1.0- 0.84- 
+00006ed0: 302e 3637 5d2c 3138 3137 2e37 352c 3138  0.67],1817.75,18
+00006ee0: 3932 2e37 352c 3139 3137 2e37 352c 3139  92.75,1917.75,19
+00006ef0: 3330 2c32 2e35 3835 3331 2c53 0d0a 3138  30,2.58531,S..18
+00006f00: 3833 312c 532c 3235 3434 352c 7965 732c  831,S,25445,yes,
+00006f10: 7965 732c 7965 732c 6e6f 2c2c 6e6f 2c79  yes,yes,no,,no,y
+00006f20: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00006f30: 2065 6e67 696e 652c 7065 7472 6f6c 2c31   engine,petrol,1
+00006f40: 3530 2c33 3130 2c72 6561 722c 2c2c 2c2c  50,310,rear,,,,,
+00006f50: 2c2c 2c2c 2c2c 312e 3330 312c 342e 3133  ,,,,,,1.301,4.13
+00006f60: 342c 322e 3433 2c31 2e38 312c 2c31 3739  4,2.43,1.81,,179
+00006f70: 362c 7265 6775 6c61 722c 342c 646f 6863  6,regular,4,dohc
+00006f80: 2c64 6972 6563 7420 696e 6a65 6374 696f  ,direct injectio
+00006f90: 6e2c 3630 2c35 3530 302c 3135 302c 3230  n,60,5500,150,20
+00006fa0: 3030 2c33 3130 2c79 6573 2c34 2c63 6162  00,310,yes,4,cab
+00006fb0: 7269 6f6c 6574 2c32 2c61 7661 696c 6162  riolet,2,availab
+00006fc0: 6c65 2c35 3232 3530 2c32 2c32 3031 322c  le,52250,2,2012,
+00006fd0: 6d61 6e75 616c 2c36 2e35 2c36 2e39 2c31  manual,6.5,6.9,1
+00006fe0: 3630 2c45 2c35 2e33 2c32 3434 2c39 2e35  60,E,5.3,244,9.5
+00006ff0: 2c33 2e32 372c 3237 3530 2c31 3337 352c  ,3.27,2750,1375,
+00007000: 3137 3930 2c35 302c 3835 2c32 3934 2e38  1790,50,85,294.8
+00007010: 3735 2c33 3037 2e39 3132 3632 3134 2c5b  75,307.9126214,[
+00007020: 342e 3436 2d20 322e 3631 2d20 312e 3732  4.46- 2.61- 1.72
+00007030: 2d20 312e 3235 2d20 312e 302d 2030 2e38  - 1.25- 1.0- 0.8
+00007040: 345d 2c31 3333 342e 352c 3134 3039 2e35  4],1334.5,1409.5
+00007050: 2c31 3433 342e 352c 3133 3630 2c32 2e33  ,1434.5,1360,2.3
+00007060: 3534 3831 2c53 0d0a 3138 3833 332c 532c  5481,S..18833,S,
+00007070: 3235 3434 372c 7965 732c 7965 732c 7965  25447,yes,yes,ye
+00007080: 732c 6e6f 2c2c 6e6f 2c79 6573 2c79 6573  s,no,,no,yes,yes
+00007090: 2c79 6573 2c2c 6675 656c 2065 6e67 696e  ,yes,,fuel engin
+000070a0: 652c 6469 6573 656c 2c31 3530 2c35 3030  e,diesel,150,500
+000070b0: 2c72 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c  ,rear,,,,,,,,,,,
+000070c0: 312e 3330 312c 342e 3133 342c 322e 3433  1.301,4.134,2.43
+000070d0: 2c31 2e38 312c 2c32 3134 332c 7061 7274  ,1.81,,2143,part
+000070e0: 6963 6c65 2066 696c 7465 722c 342c 646f  icle filter,4,do
+000070f0: 6863 2c63 6f6d 6d6f 6e20 7261 696c 2c36  hc,common rail,6
+00007100: 302c 3535 3030 2c31 3530 2c31 3630 302c  0,5500,150,1600,
+00007110: 3530 302c 7965 732c 342c 6361 6272 696f  500,yes,4,cabrio
+00007120: 6c65 742c 322c 6176 6169 6c61 626c 652c  let,2,available,
+00007130: 3530 3835 302c 322c 3230 3132 2c6d 616e  50850,2,2012,man
+00007140: 7561 6c2c 362e 352c 342e 382c 3132 342c  ual,6.5,4.8,124,
+00007150: 452c 342c 3234 342c 362e 322c 322e 3437  E,4,244,6.2,2.47
+00007160: 2c32 3030 302c 3134 3730 2c31 3838 352c  ,2000,1470,1885,
+00007170: 3530 2c39 392c 3239 312e 3134 352c 3330  50,99,291.145,30
+00007180: 362e 3734 3735 3732 382c 5b35 2e31 2d20  6.7475728,[5.1- 
+00007190: 322e 3738 2d20 312e 3735 2d20 312e 3235  2.78- 1.75- 1.25
+000071a0: 2d20 312e 302d 2030 2e38 315d 2c31 3432  - 1.0- 0.81],142
+000071b0: 392e 352c 3135 3034 2e35 2c31 3532 392e  9.5,1504.5,1529.
+000071c0: 352c 3134 3730 2c32 2e33 3534 3831 2c53  5,1470,2.35481,S
+000071d0: 0d0a 3935 3735 2c53 2c31 3138 3230 2c79  ..9575,S,11820,y
+000071e0: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+000071f0: 6e6f 2c79 6573 2c79 6573 2c79 6573 2c2c  no,yes,yes,yes,,
+00007200: 6675 656c 2065 6e67 696e 652c 7065 7472  fuel engine,petr
+00007210: 6f6c 2c31 3335 2c32 3730 2c72 6561 722c  ol,135,270,rear,
+00007220: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3239 312c  ,,,,,,,,,,1.291,
+00007230: 342e 3233 392c 322e 3439 362c 312e 3739  4.239,2.496,1.79
+00007240: 2c2c 3139 3937 2c72 6567 756c 6172 2c34  ,,1997,regular,4
+00007250: 2c64 6f68 632c 6469 7265 6374 2069 6e6a  ,dohc,direct inj
+00007260: 6563 7469 6f6e 2c35 352c 3530 3030 2c31  ection,55,5000,1
+00007270: 3335 2c31 3235 302c 3237 302c 7965 732c  35,1250,270,yes,
+00007280: 342c 6361 6272 696f 6c65 742c 322c 6176  4,cabriolet,2,av
+00007290: 6169 6c61 626c 652c 3531 3339 352c 322c  ailable,51395,2,
+000072a0: 3230 3133 2c6d 616e 7561 6c2c 362e 392c  2013,manual,6.9,
+000072b0: 362e 382c 3135 392c 452c 352e 362c 3233  6.8,159,E,5.6,23
+000072c0: 352c 382e 392c 332e 3733 2c32 3535 302c  5,8.9,3.73,2550,
+000072d0: 3133 3730 2c31 3732 352c 302c 3930 2e31  1370,1725,0,90.1
+000072e0: 2c32 3934 2e38 3735 2c33 3037 2e39 3132  ,294.875,307.912
+000072f0: 3632 3134 2c5b 332e 3638 2d20 322e 3036  6214,[3.68- 2.06
+00007300: 2d20 312e 3331 2d20 312e 302d 2030 2e38  - 1.31- 1.0- 0.8
+00007310: 312d 2030 2e36 385d 2c31 3333 322e 3837  1- 0.68],1332.87
+00007320: 352c 3134 3037 2e38 3735 2c31 3433 322e  5,1407.875,1432.
+00007330: 3837 352c 3133 3630 2c32 2e33 3130 3839  875,1360,2.31089
+00007340: 2c53 0d0a 3533 3830 2c53 2c36 3635 312c  ,S..5380,S,6651,
+00007350: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+00007360: 2c6e 6f2c 7965 732c 7965 732c 7965 732c  ,no,yes,yes,yes,
+00007370: 2c66 7565 6c20 656e 6769 6e65 2c64 6965  ,fuel engine,die
+00007380: 7365 6c2c 3133 352c 3338 302c 6672 6f6e  sel,135,380,fron
+00007390: 742c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3335  t,,,,,,,,,,,1.35
+000073a0: 352c 342e 3137 372c 322e 3530 352c 312e  5,4.177,2.505,1.
+000073b0: 3833 322c 2c31 3938 342c 7061 7274 6963  832,,1984,partic
+000073c0: 6c65 2066 696c 7465 722c 342c 646f 6863  le filter,4,dohc
+000073d0: 2c63 6f6d 6d6f 6e20 7261 696c 2c35 302c  ,common rail,50,
+000073e0: 3335 3030 2c31 3335 2c31 3735 302c 3338  3500,135,1750,38
+000073f0: 302c 7965 732c 342c 6361 6272 696f 6c65  0,yes,4,cabriole
+00007400: 742c 322c 6176 6169 6c61 626c 652c 3534  t,2,available,54
+00007410: 3331 302c 342c 3230 3135 2c6d 616e 7561  310,4,2015,manua
+00007420: 6c2c 372e 332c 342e 332c 3131 342c 442c  l,7.3,4.3,114,D,
+00007430: 332e 392c 3233 372c 352e 312c 322e 3736  3.9,237,5.1,2.76
+00007440: 2c32 3035 302c 3133 3335 2c31 3638 302c  ,2050,1335,1680,
+00007450: 3735 2c39 322e 382c 3330 332e 3635 2c33  75,92.8,303.65,3
+00007460: 3138 2e38 3334 3935 3135 2c5b 332e 3737  18.8349515,[3.77
+00007470: 2d20 322e 3039 2d20 312e 3332 2d20 302e  - 2.09- 1.32- 0.
+00007480: 3932 2d20 302e 392d 2030 2e37 365d 2c31  92- 0.9- 0.76],1
+00007490: 3330 312e 3235 2c31 3337 362e 3235 2c31  301.25,1376.25,1
+000074a0: 3430 312e 3235 2c31 3336 302c 322e 3438  401.25,1360,2.48
+000074b0: 3233 362c 530d 0a39 3933 362c 532c 3132  236,S..9936,S,12
+000074c0: 3432 392c 7965 732c 7965 732c 7965 732c  429,yes,yes,yes,
+000074d0: 6e6f 2c2c 6e6f 2c6e 6f2c 7965 732c 6e6f  no,,no,no,yes,no
+000074e0: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
+000074f0: 7472 6f6c 2c39 332c 3136 372c 7265 6172  trol,93,167,rear
+00007500: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e32 3435  ,,,,,,,,,,,1.245
+00007510: 2c34 2e30 322c 322e 3333 2c31 2e37 322c  ,4.02,2.33,1.72,
+00007520: 2c31 3739 382c 7265 6775 6c61 722c 342c  ,1798,regular,4,
+00007530: 646f 6863 2c6d 756c 7469 706f 696e 7420  dohc,multipoint 
+00007540: 696e 6a65 6374 696f 6e2c 3530 2c36 3530  injection,50,650
+00007550: 302c 3933 2c34 3530 302c 3136 372c 6e6f  0,93,4500,167,no
+00007560: 2c34 2c63 6162 7269 6f6c 6574 2c32 2c61  ,4,cabriolet,2,a
+00007570: 7661 696c 6162 6c65 2c33 3134 3930 2c32  vailable,31490,2
+00007580: 2c32 3031 342c 6d61 6e75 616c 2c39 2e39  ,2014,manual,9.9
+00007590: 2c37 2e31 2c31 3637 2c46 2c35 2e36 2c31  ,7.1,167,F,5.6,1
+000075a0: 3934 2c39 2e38 2c34 2e31 2c33 3430 302c  94,9.8,4.1,3400,
+000075b0: 3130 3530 2c31 3337 352c 2c38 332e 312c  1050,1375,,83.1,
+000075c0: 3238 372e 3835 352c 3239 392e 3137 3437  287.855,299.1747
+000075d0: 3537 332c 5b33 2e31 342d 2031 2e38 392d  573,[3.14- 1.89-
+000075e0: 2031 2e33 332d 2031 2e30 2d20 302e 3831   1.33- 1.0- 0.81
+000075f0: 5d2c 3130 3136 2e32 352c 3130 3931 2e32  ],1016.25,1091.2
+00007600: 352c 3131 3136 2e32 352c 3131 3330 2c32  5,1116.25,1130,2
+00007610: 2e31 3431 342c 530d 0a37 3939 352c 532c  .1414,S..7995,S,
+00007620: 3935 3833 2c79 6573 2c79 6573 2c34 3136  9583,yes,yes,416
+00007630: 2c6e 6f2c 2c6e 6f2c 3534 312c 7965 732c  ,no,,no,541,yes,
+00007640: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
+00007650: 2c70 6574 726f 6c2c 3234 332c 3337 302c  ,petrol,243,370,
+00007660: 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  rear,,,,,,,,,,,1
+00007670: 2e32 3733 2c34 2e34 3034 2c32 2e34 3735  .273,4.404,2.475
+00007680: 2c31 2e38 3031 2c2c 3334 3336 2c72 6567  ,1.801,,3436,reg
+00007690: 756c 6172 2c36 2c64 6f68 632c 6469 7265  ular,6,dohc,dire
+000076a0: 6374 2069 6e6a 6563 7469 6f6e 2c36 342c  ct injection,64,
+000076b0: 3637 3030 2c32 3433 2c34 3530 302c 3337  6700,243,4500,37
+000076c0: 302c 6e6f 2c34 2c63 6162 7269 6f6c 6574  0,no,4,cabriolet
+000076d0: 2c32 2c61 7661 696c 6162 6c65 2c39 3238  ,2,available,928
+000076e0: 3030 2c32 2c32 3031 342c 6175 746f 6d61  00,2,2014,automa
+000076f0: 7469 632c 342e 392c 382e 322c 3139 302c  tic,4.9,8.2,190,
+00007700: 462c 362e 332c 3237 392c 3131 2e34 2c33  F,6.3,279,11.4,3
+00007710: 2e32 352c 3139 3030 2c31 3335 302c 3136  .25,1900,1350,16
+00007720: 3835 2c37 352c 3737 2e35 2c33 3138 2e31  85,75,77.5,318.1
+00007730: 3535 2c33 3236 2e34 3536 3331 3037 2c5b  55,326.4563107,[
+00007740: 332e 3931 2d20 322e 3239 2d20 312e 3635  3.91- 2.29- 1.65
+00007750: 2d20 312e 332d 2031 2e30 382d 2030 2e38  - 1.3- 1.08- 0.8
+00007760: 382d 2030 2e36 325d 2c31 3330 362e 382c  8- 0.62],1306.8,
+00007770: 3133 3831 2e38 2c31 3430 362e 382c 3133  1381.8,1406.8,13
+00007780: 3630 2c32 2e32 3932 3637 332c 530d 0a36  60,2.292673,S..6
+00007790: 3333 312c 532c 3737 3236 2c79 6573 2c79  331,S,7726,yes,y
+000077a0: 6573 2c79 6573 2c79 6573 2c2c 6e6f 2c79  es,yes,yes,,no,y
+000077b0: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+000077c0: 2065 6e67 696e 652c 7065 7472 6f6c 2c34   engine,petrol,4
+000077d0: 3132 2c37 3535 2c72 6561 722c 2c2c 2c2c  12,755,rear,,,,,
+000077e0: 2c2c 2c2c 2c2c 312e 3332 322c 342e 3537  ,,,,,,1.322,4.57
+000077f0: 2c32 2e36 372c 312e 3931 2c2c 3338 3535  ,2.67,1.91,,3855
+00007800: 2c72 6567 756c 6172 2c38 2c64 6f68 632c  ,regular,8,dohc,
+00007810: 6469 7265 6374 2069 6e6a 6563 7469 6f6e  direct injection
+00007820: 2c37 382c 3735 3030 2c34 3132 2c34 3735  ,78,7500,412,475
+00007830: 302c 3735 352c 7965 732c 342c 6361 6272  0,755,yes,4,cabr
+00007840: 696f 6c65 742c 322c 6176 6169 6c61 626c  iolet,2,availabl
+00007850: 652c 3232 3333 3438 2c34 2c32 3031 342c  e,223348,4,2014,
+00007860: 6175 746f 6d61 7469 632c 332e 362c 3130  automatic,3.6,10
+00007870: 2e35 2c32 3530 2c47 2c2c 3331 362c 2c34  .5,250,G,,316,,4
+00007880: 2e34 342c 3330 3030 2c31 3632 352c 2c2c  .44,3000,1625,,,
+00007890: 3832 2c33 3137 2e37 342c 3332 392e 3431  82,317.74,329.41
+000078a0: 3734 3735 372c 5b33 2e34 2d20 322e 3139  74757,[3.4- 2.19
+000078b0: 2d20 312e 3633 2d20 312e 3239 2d20 312e  - 1.63- 1.29- 1.
+000078c0: 3033 2d20 302e 3834 2d20 302e 3732 5d2c  03- 0.84- 0.72],
+000078d0: 3135 3732 2e33 352c 3136 3437 2e33 352c  1572.35,1647.35,
+000078e0: 3136 3732 2e33 352c 3137 3030 2c32 2e35  1672.35,1700,2.5
+000078f0: 3235 3032 2c53 0d0a 3138 3137 332c 532c  2502,S..18173,S,
+00007900: 3234 3438 352c 7965 732c 7965 732c 6e6f  24485,yes,yes,no
+00007910: 2c79 6573 2c2c 6e6f 2c6e 6f2c 7965 732c  ,yes,,no,no,yes,
+00007920: 6e6f 2c2c 6675 656c 2065 6e67 696e 652c  no,,fuel engine,
+00007930: 7065 7472 6f6c 2c34 3139 2c35 3430 2c66  petrol,419,540,f
+00007940: 726f 6e74 2b72 6561 722c 2c2c 2c2c 2c2c  ront+rear,,,,,,,
+00007950: 2c2c 2c2c 312e 3138 342c 342e 3338 362c  ,,,,1.184,4.386,
+00007960: 322e 3536 2c31 2e39 2c2c 3532 3034 2c72  2.56,1.9,,5204,r
+00007970: 6567 756c 6172 2c31 302c 646f 6863 2c64  egular,10,dohc,d
+00007980: 6972 6563 7420 696e 6a65 6374 696f 6e2c  irect injection,
+00007990: 3830 2c38 3030 302c 3431 392c 3635 3030  80,8000,419,6500
+000079a0: 2c35 3430 2c6e 6f2c 342c 6361 6272 696f  ,540,no,4,cabrio
+000079b0: 6c65 742c 322c 3230 3133 2c33 3138 3537  let,2,2013,31857
+000079c0: 302c 322c 3230 3132 2c6d 616e 7561 6c2c  0,2,2012,manual,
+000079d0: 332e 392c 3133 2e36 2c33 3237 2c47 2c39  3.9,13.6,327,G,9
+000079e0: 2e36 2c33 3234 2c32 302e 352c 332e 3038  .6,324,20.5,3.08
+000079f0: 2c32 3435 302c 3134 3835 2c31 3830 302c  ,2450,1485,1800,
+00007a00: 2c39 322e 382c 3330 352e 3435 352c 3331  ,92.8,305.455,31
+00007a10: 342e 3132 3632 3133 362c 5b32 2e35 362d  4.1262136,[2.56-
+00007a20: 2031 2e38 352d 2031 2e34 322d 2031 2e31   1.85- 1.42- 1.1
+00007a30: 342d 2030 2e39 342d 2030 2e38 315d 2c31  4- 0.94- 0.81],1
+00007a40: 3433 312c 3135 3036 2c31 3533 312c 3134  431,1506,1531,14
+00007a50: 3730 2c32 2e32 3439 362c 530d 0a33 3432  70,2.2496,S..342
+00007a60: 3836 2c4d 2c34 3837 3431 2c79 6573 2c79  86,M,48741,yes,y
+00007a70: 6573 2c79 6573 2c79 6573 2c2c 7965 732c  es,yes,yes,,yes,
+00007a80: 7965 732c 7965 732c 7965 732c 2c66 7565  yes,yes,yes,,fue
+00007a90: 6c20 656e 6769 6e65 2c70 6574 726f 6c2c  l engine,petrol,
+00007aa0: 3835 2c31 3930 2c66 726f 6e74 2c2c 2c2c  85,190,front,,,,
+00007ab0: 2c2c 2c2c 2c2c 2c31 2e36 342c 342e 3336  ,,,,,,,1.64,4.36
+00007ac0: 362c 322e 3730 322c 312e 3834 352c 2c31  6,2.702,1.845,,1
+00007ad0: 3139 382c 7265 6775 6c61 722c 342c 646f  198,regular,4,do
+00007ae0: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
+00007af0: 696f 6e2c 3630 2c34 3530 302c 3835 2c32  ion,60,4500,85,2
+00007b00: 3030 302c 3139 302c 7965 732c 342c 6d70  000,190,yes,4,mp
+00007b10: 762c 352c 3230 3135 2c32 3736 3930 2c35  v,5,2015,27690,5
+00007b20: 2c32 3031 342c 6d61 6e75 616c 2c31 312e  ,2014,manual,11.
+00007b30: 372c 352e 392c 3133 352c 422c 352e 322c  7,5.9,135,B,5.2,
+00007b40: 3138 352c 372e 322c 342e 3733 2c33 3335  185,7.2,4.73,335
+00007b50: 302c 3132 3935 2c31 3935 352c 2c37 332e  0,1295,1955,,73.
+00007b60: 312c 3330 332e 3834 352c 3331 392e 3037  1,303.845,319.07
+00007b70: 3736 3639 392c 5b33 2e37 332d 2032 2e31  76699,[3.73- 2.1
+00007b80: 312d 2031 2e34 352d 2031 2e30 392d 2030  1- 1.45- 1.09- 0
+00007b90: 2e38 372d 2030 2e37 335d 2c31 3235 342e  .87- 0.73],1254.
+00007ba0: 352c 3133 3239 2e35 2c31 3335 342e 352c  5,1329.5,1354.5,
+00007bb0: 3133 3630 2c33 2e30 3235 382c 4d0d 0a33  1360,3.0258,M..3
+00007bc0: 3432 3739 2c4d 2c34 3837 3334 2c79 6573  4279,M,48734,yes
+00007bd0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
+00007be0: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
+00007bf0: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
+00007c00: 2c38 312c 3236 302c 6672 6f6e 742c 2c2c  ,81,260,front,,,
+00007c10: 2c2c 2c2c 2c2c 2c2c 312e 3634 2c34 2e33  ,,,,,,,,1.64,4.3
+00007c20: 3636 2c32 2e37 3032 2c31 2e38 3435 2c2c  66,2.702,1.845,,
+00007c30: 3134 3631 2c70 6172 7469 636c 6520 6669  1461,particle fi
+00007c40: 6c74 6572 2c34 2c64 6f68 632c 636f 6d6d  lter,4,dohc,comm
+00007c50: 6f6e 2072 6169 6c2c 3630 2c34 3030 302c  on rail,60,4000,
+00007c60: 3831 2c31 3735 302c 3236 302c 7965 732c  81,1750,260,yes,
+00007c70: 322c 6d70 762c 352c 6176 6169 6c61 626c  2,mpv,5,availabl
+00007c80: 652c 3330 3739 302c 352c 3230 3134 2c6d  e,30790,5,2014,m
+00007c90: 616e 7561 6c2c 3132 2e35 2c34 2e31 2c31  anual,12.5,4.1,1
+00007ca0: 3035 2c42 2c33 2e39 2c31 3830 2c34 2e35  05,B,3.9,180,4.5
+00007cb0: 2c34 2e31 332c 3235 3530 2c31 3336 302c  ,4.13,2550,1360,
+00007cc0: 3139 3637 2c2c 3830 2e35 2c32 3939 2e31  1967,,80.5,299.1
+00007cd0: 342c 3331 362e 3639 3930 3239 312c 5b33  4,316.6990291,[3
+00007ce0: 2e37 332d 2031 2e39 362d 2031 2e33 322d  .73- 1.96- 1.32-
+00007cf0: 2030 2e39 382d 2030 2e37 362d 2030 2e36   0.98- 0.76- 0.6
+00007d00: 345d 2c31 3331 392e 352c 3133 3934 2e35  4],1319.5,1394.5
+00007d10: 2c31 3431 392e 352c 3133 3630 2c33 2e30  ,1419.5,1360,3.0
+00007d20: 3235 382c 4d0d 0a32 3037 3036 2c4d 2c32  258,M..20706,M,2
+00007d30: 3831 3135 2c79 6573 2c79 6573 2c79 6573  8115,yes,yes,yes
+00007d40: 2c79 6573 2c2c 6e6f 2c35 3835 2c79 6573  ,yes,,no,585,yes
+00007d50: 2c79 6573 2c2c 6675 656c 2065 6e67 696e  ,yes,,fuel engin
+00007d60: 652c 6469 6573 656c 2c37 372c 3235 302c  e,diesel,77,250,
+00007d70: 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c 2c2c  front,,,,,,,,,,,
+00007d80: 312e 3637 342c 342e 3339 372c 322e 3637  1.674,4.397,2.67
+00007d90: 382c 312e 3739 342c 2c31 3539 382c 7061  8,1.794,,1598,pa
+00007da0: 7274 6963 6c65 2066 696c 7465 722c 342c  rticle filter,4,
+00007db0: 646f 6863 2c63 6f6d 6d6f 6e20 7261 696c  dohc,common rail
+00007dc0: 2c36 302c 3434 3030 2c37 372c 3135 3030  ,60,4400,77,1500
+00007dd0: 2c32 3530 2c79 6573 2c34 2c6d 7076 2c35  ,250,yes,4,mpv,5
+00007de0: 2c32 3031 352c 3335 3339 302c 372c 3230  ,2015,35390,7,20
+00007df0: 3134 2c6d 616e 7561 6c2c 3132 2e38 2c34  14,manual,12.8,4
+00007e00: 2e36 2c31 3231 2c45 2c34 2e31 2c31 3836  .6,121,E,4.1,186
+00007e10: 2c35 2e35 2c33 2e36 352c 3233 3030 2c31  ,5.5,3.65,2300,1
+00007e20: 3434 342c 3231 3830 2c31 3030 2c38 302e  444,2180,100,80.
+00007e30: 352c 3239 312e 3134 352c 3330 362e 3734  5,291.145,306.74
+00007e40: 3735 3732 382c 5b34 2e31 312d 2032 2e31  75728,[4.11- 2.1
+00007e50: 322d 2031 2e33 362d 2030 2e39 372d 2030  2- 1.36- 0.97- 0
+00007e60: 2e37 372d 2030 2e36 335d 2c31 3430 332e  .77- 0.63],1403.
+00007e70: 352c 3134 3738 2e35 2c31 3530 332e 352c  5,1478.5,1503.5,
+00007e80: 3134 3730 2c33 2e30 3033 3135 362c 4d0d  1470,3.003156,M.
+00007e90: 0a33 3430 3538 2c4d 2c34 3834 3934 2c79  .34058,M,48494,y
+00007ea0: 6573 2c79 6573 2c79 6573 2c79 6573 2c2c  es,yes,yes,yes,,
+00007eb0: 6e6f 2c79 6573 2c79 6573 2c6e 6f2c 2c66  no,yes,yes,no,,f
+00007ec0: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
+00007ed0: 6c2c 3131 352c 3234 302c 6672 6f6e 742c  l,115,240,front,
+00007ee0: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3633 392c  ,,,,,,,,,,1.639,
+00007ef0: 342e 3336 352c 322e 3631 332c 312e 3833  4.365,2.613,1.83
+00007f00: 372c 2c31 3539 382c 7265 6775 6c61 722c  7,,1598,regular,
+00007f10: 342c 646f 6863 2c64 6972 6563 7420 696e  4,dohc,direct in
+00007f20: 6a65 6374 696f 6e2c 3630 2c36 3030 302c  jection,60,6000,
+00007f30: 3131 352c 3134 3030 2c32 3430 2c79 6573  115,1400,240,yes
+00007f40: 2c34 2c6d 7076 2c35 2c61 7661 696c 6162  ,4,mpv,5,availab
+00007f50: 6c65 2c33 3139 3530 2c35 2c32 3031 342c  le,31950,5,2014,
+00007f60: 6d61 6e75 616c 2c38 2e39 2c36 2e39 2c31  manual,8.9,6.9,1
+00007f70: 3539 2c44 2c35 2e35 2c32 3032 2c39 2e33  59,D,5.5,202,9.3
+00007f80: 2c34 2e31 382c 3237 3530 2c31 3433 342c  ,4.18,2750,1434,
+00007f90: 3230 3230 2c37 352c 3835 2e38 2c33 3033  2020,75,85.8,303
+00007fa0: 2e36 352c 3331 382e 3833 3439 3531 352c  .65,318.8349515,
+00007fb0: 5b33 2e35 342d 2031 2e39 322d 2031 2e33  [3.54- 1.92- 1.3
+00007fc0: 332d 2031 2e30 332d 2030 2e38 322d 2030  3- 1.03- 0.82- 0
+00007fd0: 2e36 385d 2c31 3339 332e 352c 3134 3638  .68],1393.5,1468
+00007fe0: 2e35 2c31 3439 332e 352c 3134 3730 2c33  .5,1493.5,1470,3
+00007ff0: 2e30 3130 3834 332c 4d0d 0a33 3430 3537  .010843,M..34057
+00008000: 2c4d 2c34 3834 3933 2c79 6573 2c79 6573  ,M,48493,yes,yes
+00008010: 2c79 6573 2c79 6573 2c2c 6e6f 2c79 6573  ,yes,yes,,no,yes
+00008020: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
+00008030: 6e67 696e 652c 6469 6573 656c 2c38 352c  ngine,diesel,85,
+00008040: 3237 302c 6672 6f6e 742c 2c2c 2c2c 2c2c  270,front,,,,,,,
+00008050: 2c2c 2c2c 312e 3633 392c 342e 3336 352c  ,,,,1.639,4.365,
+00008060: 322e 3631 332c 312e 3833 372c 2c31 3536  2.613,1.837,,156
+00008070: 302c 7061 7274 6963 6c65 2066 696c 7465  0,particle filte
+00008080: 722c 342c 646f 6863 2c63 6f6d 6d6f 6e20  r,4,dohc,common 
+00008090: 7261 696c 2c36 302c 3336 3030 2c38 352c  rail,60,3600,85,
+000080a0: 3137 3530 2c32 3730 2c79 6573 2c34 2c6d  1750,270,yes,4,m
+000080b0: 7076 2c35 2c32 3031 342c 3332 3835 302c  pv,5,2014,32850,
+000080c0: 352c 3230 3134 2c61 7574 6f6d 6174 6963  5,2014,automatic
+000080d0: 2c31 322e 362c 342e 322c 3131 302c 432c  ,12.6,4.2,110,C,
+000080e0: 342c 3138 332c 342e 352c 342e 3138 2c32  4,183,4.5,4.18,2
+000080f0: 3435 302c 3133 3938 2c32 3032 302c 3735  450,1398,2020,75
+00008100: 2c38 382e 332c 3330 332e 3635 2c33 3138  ,88.3,303.65,318
+00008110: 2e38 3334 3935 3135 2c5b 332e 3534 2d20  .8349515,[3.54- 
+00008120: 312e 3932 2d20 312e 3332 2d20 302e 3938  1.92- 1.32- 0.98
+00008130: 2d20 302e 3736 2d20 302e 365d 2c31 3335  - 0.76- 0.6],135
+00008140: 372e 352c 3134 3332 2e35 2c31 3435 372e  7.5,1432.5,1457.
+00008150: 352c 3134 3730 2c33 2e30 3130 3834 332c  5,1470,3.010843,
+00008160: 4d0d 0a32 3432 3638 2c4d 2c33 3431 3034  M..24268,M,34104
+00008170: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
+00008180: 2c2c 7965 732c 7965 732c 7965 732c 6e6f  ,,yes,yes,yes,no
+00008190: 2c2c 6675 656c 2065 6e67 696e 652c 7065  ,,fuel engine,pe
+000081a0: 7472 6f6c 2c31 3138 2c32 3430 2c66 726f  trol,118,240,fro
+000081b0: 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e36  nt,,,,,,,,,,,1.6
+000081c0: 3538 2c34 2e37 3638 2c32 2e38 352c 312e  58,4.768,2.85,1.
+000081d0: 3838 342c 2c31 3539 362c 7265 6775 6c61  884,,1596,regula
+000081e0: 722c 342c 646f 6863 2c64 6972 6563 7420  r,4,dohc,direct 
+000081f0: 696e 6a65 6374 696f 6e2c 3730 2c35 3730  injection,70,570
+00008200: 302c 3131 382c 3137 3530 2c32 3430 2c79  0,118,1750,240,y
+00008210: 6573 2c34 2c6d 7076 2c35 2c61 7661 696c  es,4,mpv,5,avail
+00008220: 6162 6c65 2c33 3938 3835 2c30 352d 4a75  able,39885,05-Ju
+00008230: 6c2c 3230 3133 2c6d 616e 7561 6c2c 392e  l,2013,manual,9.
+00008240: 382c 372c 3135 392c 432c 352e 372c 3230  8,7,159,C,5.7,20
+00008250: 342c 392e 342c 342e 3037 2c2c 3134 3938  4,9.4,4.07,,1498
+00008260: 2c32 3430 302c 3735 2c38 312e 342c 3330  ,2400,75,81.4,30
+00008270: 332e 3635 2c33 3138 2e38 3334 3935 3135  3.65,318.8349515
+00008280: 2c5b 332e 382d 2032 2e31 342d 2031 2e34  ,[3.8- 2.14- 1.4
+00008290: 382d 2031 2e31 312d 2030 2e39 5d2c 3134  8- 1.11- 0.9],14
+000082a0: 3530 2e37 352c 3135 3235 2e37 352c 3135  50.75,1525.75,15
+000082b0: 3530 2e37 352c 3134 3730 2c33 2e31 3233  50.75,1470,3.123
+000082c0: 3637 322c 4d0d 0a31 3930 3238 2c4d 2c32  672,M..19028,M,2
+000082d0: 3537 3334 2c79 6573 2c79 6573 2c79 6573  5734,yes,yes,yes
+000082e0: 2c6e 6f2c 2c6e 6f2c 6e6f 2c79 6573 2c79  ,no,,no,no,yes,y
+000082f0: 6573 2c2c 6675 656c 2065 6e67 696e 652c  es,,fuel engine,
+00008300: 7065 7472 6f6c 2c31 3033 2c32 3030 2c66  petrol,103,200,f
+00008310: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
+00008320: 2e36 3835 2c34 2e36 3538 2c32 2e37 362c  .685,4.658,2.76,
+00008330: 312e 3832 2c2c 3133 3634 2c72 6567 756c  1.82,,1364,regul
+00008340: 6172 2c34 2c64 6f68 632c 6d75 6c74 6970  ar,4,dohc,multip
+00008350: 6f69 6e74 2069 6e6a 6563 7469 6f6e 2c35  oint injection,5
+00008360: 382c 3439 3030 2c31 3033 2c31 3835 302c  8,4900,103,1850,
+00008370: 3230 302c 7965 732c 342c 6d70 762c 352c  200,yes,4,mpv,5,
+00008380: 6176 6169 6c61 626c 652c 3238 3139 352c  available,28195,
+00008390: 3035 2d4a 756c 2c32 3031 352c 6d61 6e75  05-Jul,2015,manu
 000083a0: 616c 2c31 302e 372c 362e 312c 3134 342c  al,10.7,6.1,144,
 000083b0: 432c 352e 332c 3230 322c 372e 362c 332e  C,5.3,202,7.6,3.
 000083c0: 3833 2c32 3935 302c 3135 3133 2c32 3239  83,2950,1513,229
 000083d0: 352c 2c38 322e 362c 3330 332e 3635 2c33  5,,82.6,303.65,3
 000083e0: 3138 2e38 3334 3935 3135 2c5b 342e 3237  18.8349515,[4.27
 000083f0: 2d20 322e 3335 2d20 312e 3537 2d20 312e  - 2.35- 1.57- 1.
 00008400: 3135 2d20 302e 3934 2d20 302e 385d 2c31  15- 0.94- 0.8],1
@@ -2121,376 +2121,551 @@
 00008480: 726f 6e74 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  ront,,,,,,,,,,,1
 00008490: 2e36 3835 2c34 2e36 3538 2c32 2e37 362c  .685,4.658,2.76,
 000084a0: 312e 3832 2c2c 3139 3536 2c70 6172 7469  1.82,,1956,parti
 000084b0: 636c 6520 6669 6c74 6572 2c34 2c64 6f68  cle filter,4,doh
 000084c0: 632c 636f 6d6d 6f6e 2072 6169 6c2c 3538  c,common rail,58
 000084d0: 2c33 3735 302c 3132 352c 3137 3530 2c34  ,3750,125,1750,4
 000084e0: 3030 2c79 6573 2c34 2c6d 7076 2c35 2c61  00,yes,4,mpv,5,a
-000084f0: 7661 696c 6162 6c65 2c33 3836 3435 2c35  vailable,38645,5
-00008500: 2d4a 756c 2c32 3031 352c 6d61 6e75 616c  -Jul,2015,manual
-00008510: 2c39 2e38 2c34 2e39 2c31 3239 2c44 2c34  ,9.8,4.9,129,D,4
-00008520: 2e32 2c32 3038 2c36 2e31 2c33 2e33 352c  .2,208,6.1,3.35,
-00008530: 3230 3030 2c31 3633 332c 3234 3130 2c2c  2000,1633,2410,,
-00008540: 3930 2e34 2c33 3033 2e36 352c 3331 382e  90.4,303.65,318.
-00008550: 3833 3439 3531 352c 5b34 2e31 372d 2032  8349515,[4.17- 2
-00008560: 2e31 332d 2031 2e33 322d 2030 2e39 352d  .13- 1.32- 0.95-
-00008570: 2030 2e37 362d 2030 2e36 325d 2c31 3539   0.76- 0.62],159
-00008580: 332e 3835 2c31 3636 382e 3835 2c31 3639  3.85,1668.85,169
-00008590: 332e 3835 2c31 3730 302c 332e 3036 3637  3.85,1700,3.0667
-000085a0: 2c4d 0d0a 3739 3739 2c4d 2c39 3536 352c  ,M..7979,M,9565,
-000085b0: 7965 732c 7965 732c 7965 732c 6e6f 2c2c  yes,yes,yes,no,,
-000085c0: 6e6f 2c35 3235 2c79 6573 2c6e 6f2c 2c66  no,525,yes,no,,f
-000085d0: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
-000085e0: 6c2c 3838 2c31 3630 2c66 726f 6e74 2c2c  l,88,160,front,,
-000085f0: 2c2c 2c2c 2c2c 2c2c 2c31 2e38 3031 2c34  ,,,,,,,,,1.801,4
-00008600: 2e33 382c 322e 3732 382c 312e 3831 2c2c  .38,2.728,1.81,,
-00008610: 3135 3938 2c72 6567 756c 6172 2c34 2c6f  1598,regular,4,o
-00008620: 6863 2c6d 756c 7469 706f 696e 7420 696e  hc,multipoint in
-00008630: 6a65 6374 696f 6e2c 3630 2c36 3030 302c  jection,60,6000,
-00008640: 3838 2c34 3235 302c 3136 302c 6e6f 2c34  88,4250,160,no,4
-00008650: 2c6d 7076 2c35 2c61 7661 696c 6162 6c65  ,mpv,5,available
-00008660: 2c32 3831 3530 2c35 2c32 3031 332c 6d61  ,28150,5,2013,ma
-00008670: 6e75 616c 2c31 322c 372e 332c 3136 392c  nual,12,7.3,169,
-00008680: 452c 362c 3137 372c 392e 362c 352e 3037  E,6,177,9.6,5.07
-00008690: 2c33 3730 302c 3132 3935 2c32 3030 302c  ,3700,1295,2000,
-000086a0: 3130 302c 3835 2e35 2c32 3934 2e34 3335  100,85.5,294.435
-000086b0: 2c33 3134 2e33 3230 3338 3833 2c5b 332e  ,314.3203883,[3.
-000086c0: 3435 2d20 312e 3837 2d20 312e 3239 2d20  45- 1.87- 1.29- 
-000086d0: 302e 3935 2d20 302e 3734 5d2c 3132 3534  0.95- 0.74],1254
-000086e0: 2e35 2c31 3332 392e 352c 3133 3534 2e35  .5,1329.5,1354.5
-000086f0: 2c31 3336 302c 332e 3235 3938 312c 4d0d  ,1360,3.25981,M.
-00008700: 0a32 3235 3931 2c4a 2c33 3132 3035 2c79  .22591,J,31205,y
-00008710: 6573 2c79 6573 2c79 6573 2c6e 6f2c 2c34  es,yes,yes,no,,4
-00008720: 3530 2c79 6573 2c79 6573 2c6e 6f2c 2c66  50,yes,yes,no,,f
-00008730: 7565 6c20 656e 6769 6e65 2c64 6965 7365  uel engine,diese
-00008740: 6c2c 3133 302c 3335 302c 6672 6f6e 742b  l,130,350,front+
-00008750: 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  rear,,,,,,,,,,,1
-00008760: 2e37 3033 2c34 2e34 3236 2c32 2e36 3034  .703,4.426,2.604
-00008770: 2c31 2e38 3039 2c2c 3139 3638 2c70 6172  ,1.809,,1968,par
-00008780: 7469 636c 6520 6669 6c74 6572 2c34 2c64  ticle filter,4,d
-00008790: 6f68 632c 636f 6d6d 6f6e 2072 6169 6c2c  ohc,common rail,
-000087a0: 3634 2c34 3230 302c 3133 302c 3137 3530  64,4200,130,1750
-000087b0: 2c33 3530 2c79 6573 2c34 2c73 7576 2f63  ,350,yes,4,suv/c
-000087c0: 726f 7373 6f76 6572 2c35 2c61 7661 696c  rossover,5,avail
-000087d0: 6162 6c65 2c34 3939 3930 2c35 2c32 3031  able,49990,5,201
-000087e0: 332c 6d61 6e75 616c 2c38 2e35 2c35 2e38  3,manual,8.5,5.8
-000087f0: 2c31 3531 2c47 2c35 2e32 2c32 3032 2c36  ,151,G,5.2,202,6
-00008800: 2e37 2c33 2e30 352c 3231 3530 2c31 3537  .7,3.05,2150,157
-00008810: 382c 3232 3430 2c37 352c 3935 2e35 2c33  8,2240,75,95.5,3
-00008820: 3136 2e37 3135 2c33 3335 2e30 3937 3038  16.715,335.09708
-00008830: 3734 2c5b 332e 3932 2d20 322e 3035 2d20  74,[3.92- 2.05- 
-00008840: 312e 3735 2d20 312e 3233 2d20 302e 3934  1.75- 1.23- 0.94
-00008850: 2d20 302e 3737 5d2c 3135 3334 2e38 2c31  - 0.77],1534.8,1
-00008860: 3630 392e 382c 3136 3334 2e38 2c31 3539  609.8,1634.8,159
-00008870: 302c 332e 3038 3037 3237 2c4a 0d0a 3334  0,3.080727,J..34
-00008880: 3230 322c 4a2c 3438 3635 322c 7965 732c  202,J,48652,yes,
-00008890: 7965 732c 7965 732c 6e6f 2c2c 7965 732c  yes,yes,no,,yes,
-000088a0: 7965 732c 7965 732c 6e6f 2c2c 6675 656c  yes,yes,no,,fuel
-000088b0: 2065 6e67 696e 652c 7065 7472 6f6c 2c38   engine,petrol,8
-000088c0: 382c 3139 302c 6672 6f6e 742c 2c2c 2c2c  8,190,front,,,,,
-000088d0: 2c2c 2c2c 2c2c 312e 3536 362c 342e 3132  ,,,,,,1.566,4.12
-000088e0: 322c 322e 3630 362c 312e 3737 382c 2c31  2,2.606,1.778,,1
-000088f0: 3139 362c 7265 6775 6c61 722c 342c 646f  196,regular,4,do
-00008900: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-00008910: 696f 6e2c 3435 2c34 3930 302c 3838 2c32  ion,45,4900,88,2
-00008920: 3030 302c 3139 302c 7965 732c 342c 7375  000,190,yes,4,su
-00008930: 762f 6372 6f73 736f 7665 722c 352c 6176  v/crossover,5,av
-00008940: 6169 6c61 626c 652c 3235 3139 302c 352c  ailable,25190,5,
-00008950: 3230 3135 2c61 7574 6f6d 6174 6963 2c31  2015,automatic,1
-00008960: 302e 392c 352e 342c 3132 352c 422c 342e  0.9,5.4,125,B,4.
-00008970: 372c 3139 322c 362e 362c 332e 3935 2c32  7,192,6.6,3.95,2
-00008980: 3635 302c 3131 3535 2c31 3732 362c 2c37  650,1155,1726,,7
-00008990: 332e 312c 3330 332e 3834 352c 3331 392e  3.1,303.845,319.
-000089a0: 3037 3736 3639 392c 5b33 2e39 322d 2032  0776699,[3.92- 2
-000089b0: 2e34 332d 2031 2e34 342d 2031 2e30 322d  .43- 1.44- 1.02-
-000089c0: 2030 2e38 372d 2030 2e37 5d2c 3131 3234   0.87- 0.7],1124
-000089d0: 2e36 3235 2c31 3139 392e 3632 352c 3132  .625,1199.625,12
-000089e0: 3234 2e36 3235 2c31 3235 302c 322e 3738  24.625,1250,2.78
-000089f0: 3433 3438 2c4a 0d0a 3430 3137 302c 4a2c  4348,J..40170,J,
-00008a00: 3537 3134 382c 7965 732c 7965 732c 7965  57148,yes,yes,ye
-00008a10: 732c 7965 732c 2c79 6573 2c79 6573 2c79  s,yes,,yes,yes,y
-00008a20: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
-00008a30: 696e 652c 7065 7472 6f6c 2c38 352c 3139  ine,petrol,85,19
-00008a40: 302c 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c  0,front,,,,,,,,,
-00008a50: 2c2c 312e 3539 2c34 2e33 3737 2c32 2e36  ,,1.59,4.377,2.6
-00008a60: 3436 2c31 2e38 3036 2c2c 3131 3937 2c72  46,1.806,,1197,r
-00008a70: 6567 756c 6172 2c34 2c64 6f68 632c 6469  egular,4,dohc,di
-00008a80: 7265 6374 2069 6e6a 6563 7469 6f6e 2c35  rect injection,5
-00008a90: 352c 3435 3030 2c38 352c 3230 3030 2c31  5,4500,85,2000,1
-00008aa0: 3930 2c79 6573 2c34 2c73 7576 2f63 726f  90,yes,4,suv/cro
-00008ab0: 7373 6f76 6572 2c35 2c32 3031 352c 3330  ssover,5,2015,30
-00008ac0: 3139 302c 352c 3230 3134 2c6d 616e 7561  190,5,2014,manua
-00008ad0: 6c2c 3131 2e33 2c35 2e38 2c31 3239 2c42  l,11.3,5.8,129,B
-00008ae0: 2c34 2e39 2c31 3833 2c36 2e39 2c34 2e32  ,4.9,183,6.9,4.2
-00008af0: 312c 3235 3030 2c31 3235 302c 3138 3630  1,2500,1250,1860
-00008b00: 2c37 352c 3733 2e31 2c33 3230 2e32 3735  ,75,73.1,320.275
-00008b10: 2c33 3332 2e35 3732 3831 3535 2c5b 332e  ,332.5728155,[3.
-00008b20: 3733 2d20 312e 3935 2d20 312e 3332 2d20  73- 1.95- 1.32- 
-00008b30: 302e 3938 2d20 302e 3736 2d20 302e 3634  0.98- 0.76- 0.64
-00008b40: 5d2c 3132 3132 2e38 3735 2c31 3238 372e  ],1212.875,1287.
-00008b50: 3837 352c 3133 3132 2e38 3735 2c31 3235  875,1312.875,125
-00008b60: 302c 322e 3837 3135 342c 4a0d 0a34 3435  0,2.87154,J..445
-00008b70: 3939 2c4a 2c36 3334 3832 2c79 6573 2c79  99,J,63482,yes,y
-00008b80: 6573 2c79 6573 2c79 6573 2c2c 7965 732c  es,yes,yes,,yes,
-00008b90: 7965 732c 7965 732c 7965 732c 2c66 7565  yes,yes,yes,,fue
-00008ba0: 6c20 656e 6769 6e65 2c64 6965 7365 6c2c  l engine,diesel,
-00008bb0: 3936 2c33 3230 2c66 726f 6e74 2c2c 2c2c  96,320,front,,,,
-00008bc0: 2c2c 2c2c 2c2c 2c31 2e35 392c 342e 3337  ,,,,,,,1.59,4.37
-00008bd0: 372c 322e 3634 362c 312e 3830 362c 2c31  7,2.646,1.806,,1
-00008be0: 3539 382c 7061 7274 6963 6c65 2066 696c  598,particle fil
-00008bf0: 7465 722c 342c 646f 6863 2c63 6f6d 6d6f  ter,4,dohc,commo
-00008c00: 6e20 7261 696c 2c35 352c 3430 3030 2c39  n rail,55,4000,9
-00008c10: 362c 3137 3530 2c33 3230 2c79 6573 2c34  6,1750,320,yes,4
-00008c20: 2c73 7576 2f63 726f 7373 6f76 6572 2c35  ,suv/crossover,5
-00008c30: 2c61 7661 696c 6162 6c65 2c33 3535 3030  ,available,35500
-00008c40: 2c35 2c32 3031 342c 6d61 6e75 616c 2c31  ,5,2014,manual,1
-00008c50: 302e 352c 342e 342c 3131 352c 442c 332e  0.5,4.4,115,D,3.
-00008c60: 392c 3139 302c 352e 322c 342e 3133 2c32  9,190,5.2,4.13,2
-00008c70: 3330 302c 3133 3430 2c31 3936 302c 3735  300,1340,1960,75
-00008c80: 2c37 392e 352c 3332 302e 3237 352c 3333  ,79.5,320.275,33
-00008c90: 322e 3537 3238 3135 352c 5b33 2e37 332d  2.5728155,[3.73-
-00008ca0: 2032 2e30 342d 2031 2e33 322d 2030 2e39   2.04- 1.32- 0.9
-00008cb0: 352d 2030 2e37 322d 2030 2e36 5d2c 3133  5- 0.72- 0.6],13
-00008cc0: 3032 2e38 3735 2c31 3337 372e 3837 352c  02.875,1377.875,
-00008cd0: 3134 3032 2e38 3735 2c31 3336 302c 322e  1402.875,1360,2.
-00008ce0: 3837 3135 342c 4a0d 0a35 3335 382c 4a2c  87154,J..5358,J,
-00008cf0: 3636 3239 2c79 6573 2c79 6573 2c79 6573  6629,yes,yes,yes
-00008d00: 2c79 6573 2c2c 7965 732c 7965 732c 7965  ,yes,,yes,yes,ye
-00008d10: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00008d20: 6e65 2c70 6574 726f 6c2c 3136 322c 3335  ne,petrol,162,35
-00008d30: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00008d40: 2c2c 2c2c 2c2c 2c31 2e36 3038 2c34 2e33  ,,,,,,,1.608,4.3
-00008d50: 3838 2c32 2e36 3033 2c31 2e38 3331 2c2c  88,2.603,1.831,,
-00008d60: 3139 3834 2c72 6567 756c 6172 2c34 2c64  1984,regular,4,d
-00008d70: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
-00008d80: 7469 6f6e 2c36 342c 3435 3030 2c31 3632  tion,64,4500,162
-00008d90: 2c31 3530 302c 3335 302c 7965 732c 342c  ,1500,350,yes,4,
-00008da0: 7375 762f 6372 6f73 736f 7665 722c 352c  suv/crossover,5,
-00008db0: 6176 6169 6c61 626c 652c 3532 3730 302c  available,52700,
-00008dc0: 352c 3230 3135 2c61 7574 6f6d 6174 6963  5,2015,automatic
-00008dd0: 2c36 2e34 2c36 2e37 2c31 3534 2c44 2c35  ,6.4,6.7,154,D,5
-00008de0: 2e39 2c32 3333 2c38 2e31 2c33 2e39 342c  .9,233,8.1,3.94,
-00008df0: 3233 3030 2c31 3534 302c 3231 3635 2c37  2300,1540,2165,7
-00008e00: 352c 3932 2e38 2c33 3136 2e37 3135 2c33  5,92.8,316.715,3
-00008e10: 3335 2e30 3937 3038 3734 2c5b 332e 3536  35.0970874,[3.56
-00008e20: 2d20 322e 3533 2d20 312e 3638 2d20 312e  - 2.53- 1.68- 1.
-00008e30: 3032 2d20 302e 3739 2d20 302e 3736 2d20  02- 0.79- 0.76- 
-00008e40: 302e 3634 5d2c 3134 3936 2e38 2c31 3537  0.64],1496.8,157
-00008e50: 312e 382c 3135 3936 2e38 2c31 3539 302c  1.8,1596.8,1590,
-00008e60: 322e 3934 3432 3438 2c4a 0d0a 3533 3338  2.944248,J..5338
-00008e70: 2c4a 2c36 3630 392c 7965 732c 7965 732c  ,J,6609,yes,yes,
-00008e80: 7965 732c 7965 732c 2c79 6573 2c79 6573  yes,yes,,yes,yes
-00008e90: 2c79 6573 2c79 6573 2c2c 6675 656c 2065  ,yes,yes,,fuel e
-00008ea0: 6e67 696e 652c 6469 6573 656c 2c31 3335  ngine,diesel,135
-00008eb0: 2c33 3830 2c66 726f 6e74 2b72 6561 722c  ,380,front+rear,
-00008ec0: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3630 382c  ,,,,,,,,,,1.608,
-00008ed0: 342e 3338 382c 322e 3630 332c 312e 3833  4.388,2.603,1.83
-00008ee0: 312c 2c31 3936 382c 7061 7274 6963 6c65  1,,1968,particle
-00008ef0: 2066 696c 7465 722c 342c 646f 6863 2c63   filter,4,dohc,c
-00008f00: 6f6d 6d6f 6e20 7261 696c 2c36 342c 3335  ommon rail,64,35
-00008f10: 3030 2c31 3335 2c31 3830 302c 3338 302c  00,135,1800,380,
-00008f20: 7965 732c 342c 7375 762f 6372 6f73 736f  yes,4,suv/crosso
-00008f30: 7665 722c 352c 6176 6169 6c61 626c 652c  ver,5,available,
-00008f40: 3531 3536 302c 352c 3230 3135 2c6d 616e  51560,5,2015,man
-00008f50: 7561 6c2c 372e 392c 352e 322c 3133 372c  ual,7.9,5.2,137,
-00008f60: 462c 342e 352c 3231 392c 362e 352c 332e  F,4.5,219,6.5,3.
-00008f70: 3337 2c32 3430 302c 3135 3830 2c32 3230  37,2400,1580,220
-00008f80: 352c 3735 2c39 352e 352c 3331 362e 3731  5,75,95.5,316.71
-00008f90: 352c 3333 352e 3039 3730 3837 342c 5b33  5,335.0970874,[3
-00008fa0: 2e39 322d 2032 2e30 352d 2031 2e37 352d  .92- 2.05- 1.75-
-00008fb0: 2031 2e32 332d 2030 2e39 342d 2030 2e37   1.23- 0.94- 0.7
-00008fc0: 375d 2c31 3533 362e 382c 3136 3131 2e38  7],1536.8,1611.8
-00008fd0: 2c31 3633 362e 382c 3135 3930 2c32 2e39  ,1636.8,1590,2.9
-00008fe0: 3434 3234 382c 4a0d 0a33 3430 3135 2c4a  44248,J..34015,J
-00008ff0: 2c34 3834 3530 2c79 6573 2c79 6573 2c79  ,48450,yes,yes,y
-00009000: 6573 2c79 6573 2c2c 6e6f 2c79 6573 2c79  es,yes,,no,yes,y
-00009010: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
-00009020: 696e 652c 6469 6573 656c 2c38 382c 3330  ine,diesel,88,30
-00009030: 302c 6672 6f6e 742c 2c2c 2c2c 2c2c 2c2c  0,front,,,,,,,,,
-00009040: 2c2c 312e 3535 362c 342e 3135 392c 322e  ,,1.556,4.159,2.
-00009050: 3533 382c 312e 3733 392c 2c31 3536 302c  538,1.739,,1560,
-00009060: 7265 6775 6c61 722c 342c 646f 6863 2c63  regular,4,dohc,c
-00009070: 6f6d 6d6f 6e20 7261 696c 2c35 302c 3335  ommon rail,50,35
-00009080: 3030 2c38 382c 3137 3530 2c33 3030 2c79  00,88,1750,300,y
-00009090: 6573 2c34 2c73 7576 2f63 726f 7373 6f76  es,4,suv/crossov
-000090a0: 6572 2c35 2c61 7661 696c 6162 6c65 2c32  er,5,available,2
-000090b0: 3637 3530 2c35 2c32 3031 352c 6d61 6e75  6750,5,2015,manu
-000090c0: 616c 2c31 302e 342c 332e 372c 3936 2c43  al,10.4,3.7,96,C
-000090d0: 2c33 2e33 2c31 3932 2c34 2e33 2c33 2e37  ,3.3,192,4.3,3.7
-000090e0: 342c 3232 3530 2c31 3137 352c 3137 3236  4,2250,1175,1726
-000090f0: 2c2c 3838 2e33 2c32 3934 2e34 362c 3331  ,,88.3,294.46,31
-00009100: 302e 3837 3337 3836 342c 5b33 2e38 352d  0.8737864,[3.85-
-00009110: 2032 2e30 392d 2031 2e33 392d 2030 2e39   2.09- 1.39- 0.9
-00009120: 392d 2030 2e37 332d 2030 2e36 315d 2c31  9- 0.73- 0.61],1
-00009130: 3134 312e 3235 2c31 3231 362e 3235 2c31  141.25,1216.25,1
-00009140: 3234 312e 3235 2c31 3235 302c 322e 3730  241.25,1250,2.70
-00009150: 3538 3834 2c4a 0d0a 3938 3732 2c4a 2c31  5884,J..9872,J,1
-00009160: 3232 3737 2c79 6573 2c79 6573 2c79 6573  2277,yes,yes,yes
-00009170: 2c79 6573 2c2c 7965 732c 7965 732c 7965  ,yes,,yes,yes,ye
-00009180: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00009190: 6e65 2c70 6574 726f 6c2c 3337 352c 3632  ne,petrol,375,62
-000091a0: 352c 6672 6f6e 742b 7265 6172 2c2c 2c2c  5,front+rear,,,,
-000091b0: 2c2c 2c2c 2c2c 2c31 2e38 3335 2c34 2e39  ,,,,,,,1.835,4.9
-000091c0: 3939 2c32 2e39 3232 2c31 2e39 3833 2c2c  99,2.922,1.983,,
-000091d0: 3530 3030 2c72 6567 756c 6172 2c38 2c64  5000,regular,8,d
-000091e0: 6f68 632c 6d75 6c74 6970 6f69 6e74 2069  ohc,multipoint i
-000091f0: 6e6a 6563 7469 6f6e 2c31 3035 2c36 3030  njection,105,600
-00009200: 302c 3337 352c 3235 3030 2c36 3235 2c79  0,375,2500,625,y
-00009210: 6573 2c34 2c73 7576 2f63 726f 7373 6f76  es,4,suv/crossov
-00009220: 6572 2c35 2c61 7661 696c 6162 6c65 2c32  er,5,available,2
-00009230: 3335 3730 302c 352c 3230 3134 2c61 7574  35700,5,2014,aut
-00009240: 6f6d 6174 6963 2c35 2e34 2c31 322e 382c  omatic,5.4,12.8,
-00009250: 3239 392c 472c 392e 372c 3232 352c 3138  299,G,9.7,225,18
-00009260: 2e33 2c33 2e33 312c 3138 3030 2c32 3333  .3,3.31,1800,233
-00009270: 302c 3331 3530 2c31 3030 2c39 332c 3336  0,3150,100,93,36
-00009280: 332e 3339 352c 3338 322e 3736 3639 3930  3.395,382.766990
-00009290: 332c 5b34 2e37 2d20 332e 3133 2d20 322e  3,[4.7- 3.13- 2.
-000092a0: 312d 2031 2e36 372d 2031 2e32 392d 2031  1- 1.67- 1.29- 1
-000092b0: 2e30 2d20 302e 3834 2d20 302e 3637 5d2c  .0- 0.84- 0.67],
-000092c0: 3232 3539 2e31 3235 2c32 3333 342e 3132  2259.125,2334.12
-000092d0: 352c 3233 3539 2e31 3235 2c32 3237 302c  5,2359.125,2270,
-000092e0: 332e 3633 3838 3035 2c4a 0d0a 3938 3536  3.638805,J..9856
-000092f0: 2c4a 2c31 3232 3631 2c79 6573 2c79 6573  ,J,12261,yes,yes
-00009300: 2c79 6573 2c79 6573 2c2c 7965 732c 7965  ,yes,yes,,yes,ye
-00009310: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
-00009320: 656e 6769 6e65 2c64 6965 7365 6c2c 3139  engine,diesel,19
-00009330: 302c 3630 302c 6672 6f6e 742b 7265 6172  0,600,front+rear
-00009340: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e38 342c  ,,,,,,,,,,,1.84,
-00009350: 352e 3139 392c 332e 3132 2c31 2e39 3833  5.199,3.12,1.983
-00009360: 2c2c 3239 3933 2c70 6172 7469 636c 6520  ,,2993,particle 
-00009370: 6669 6c74 6572 2c36 2c64 6f68 632c 636f  filter,6,dohc,co
-00009380: 6d6d 6f6e 2072 6169 6c2c 3835 2c34 3030  mmon rail,85,400
-00009390: 302c 3139 302c 3230 3030 2c36 3030 2c79  0,190,2000,600,y
-000093a0: 6573 2c34 2c73 7576 2f63 726f 7373 6f76  es,4,suv/crossov
-000093b0: 6572 2c35 2c61 7661 696c 6162 6c65 2c31  er,5,available,1
-000093c0: 3438 3530 302c 352c 3230 3134 2c61 7574  48500,5,2014,aut
-000093d0: 6f6d 6174 6963 2c37 2e39 2c36 2e39 2c31  omatic,7.9,6.9,1
-000093e0: 3832 2c43 2c36 2e33 2c32 3130 2c37 2e38  82,C,6.3,210,7.8
-000093f0: 2c33 2e32 312c 3137 3530 2c32 3330 312c  ,3.21,1750,2301,
-00009400: 3330 3530 2c31 3030 2c39 302c 3336 332e  3050,100,90,363.
-00009410: 3339 352c 3338 322e 3736 3639 3930 332c  395,382.7669903,
-00009420: 5b34 2e37 2d20 332e 3133 2d20 322e 312d  [4.7- 3.13- 2.1-
-00009430: 2031 2e36 372d 2031 2e32 392d 2031 2e30   1.67- 1.29- 1.0
-00009440: 2d20 302e 3834 2d20 302e 3637 5d2c 3232  - 0.84- 0.67],22
-00009450: 3433 2e36 3235 2c32 3331 382e 3632 352c  43.625,2318.625,
-00009460: 3233 3433 2e36 3235 2c32 3237 302c 332e  2343.625,2270,3.
-00009470: 3634 3837 322c 4a0d 0a36 3434 362c 4a2c  64872,J..6446,J,
-00009480: 3739 3239 2c79 6573 2c79 6573 2c79 6573  7929,yes,yes,yes
-00009490: 2c79 6573 2c2c 3636 302c 7965 732c 7965  ,yes,,660,yes,ye
-000094a0: 732c 6e6f 2c2c 6675 656c 2065 6e67 696e  s,no,,fuel engin
-000094b0: 652c 7065 7472 6f6c 2c31 3737 2c33 3430  e,petrol,177,340
-000094c0: 2c66 726f 6e74 2b72 6561 722c 2c2c 2c2c  ,front+rear,,,,,
-000094d0: 2c2c 2c2c 2c2c 312e 3732 342c 342e 3539  ,,,,,,1.724,4.59
-000094e0: 392c 322e 3734 312c 312e 3839 352c 2c31  9,2.741,1.895,,1
-000094f0: 3939 392c 7265 6775 6c61 722c 342c 646f  999,regular,4,do
-00009500: 6863 2c6d 756c 7469 706f 696e 7420 696e  hc,multipoint in
-00009510: 6a65 6374 696f 6e2c 3730 2c35 3530 302c  jection,70,5500,
-00009520: 3137 372c 3137 3530 2c33 3430 2c79 6573  177,1750,340,yes
-00009530: 2c34 2c73 7576 2f63 726f 7373 6f76 6572  ,4,suv/crossover
-00009540: 2c35 2c61 7661 696c 6162 6c65 2c37 3332  ,5,available,732
-00009550: 3030 2c35 2c32 3031 342c 6175 746f 6d61  00,5,2014,automa
-00009560: 7469 632c 382e 322c 382e 322c 3139 312c  tic,8.2,8.2,191,
-00009570: 452c 2c31 3939 2c2c 332e 3735 2c2c 3137  E,,199,,3.75,,17
-00009580: 3434 2c32 3530 352c 3735 2c38 332e 312c  44,2505,75,83.1,
-00009590: 3334 322e 3131 352c 3335 392e 3735 3732  342.115,359.7572
-000095a0: 3831 362c 5b34 2e31 352d 2032 2e33 372d  816,[4.15- 2.37-
-000095b0: 2031 2e35 362d 2031 2e31 362d 2030 2e38   1.56- 1.16- 0.8
-000095c0: 362d 2030 2e36 395d 2c31 3639 362e 3735  6- 0.69],1696.75
-000095d0: 2c31 3737 312e 3735 2c31 3739 362e 3735  ,1771.75,1796.75
-000095e0: 2c31 3831 302c 332e 3236 3639 382c 4a0d  ,1810,3.26698,J.
-000095f0: 0a38 3836 362c 4a2c 3131 3031 332c 7965  .8866,J,11013,ye
-00009600: 732c 7965 732c 3434 302c 6e6f 2c2c 6e6f  s,yes,440,no,,no
-00009610: 2c34 3130 2c79 6573 2c79 6573 2c2c 6675  ,410,yes,yes,,fu
-00009620: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
-00009630: 2c31 3130 2c34 3230 2c66 726f 6e74 2b72  ,110,420,front+r
-00009640: 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e  ear,,,,,,,,,,,1.
-00009650: 3734 2c34 2e35 2c32 2e36 362c 312e 3931  74,4.5,2.66,1.91
-00009660: 2c2c 3231 3739 2c70 6172 7469 636c 6520  ,,2179,particle 
-00009670: 6669 6c74 6572 2c34 2c64 6f68 632c 636f  filter,4,dohc,co
-00009680: 6d6d 6f6e 2072 6169 6c2c 3638 2c34 3030  mmon rail,68,400
-00009690: 302c 3131 302c 3137 3530 2c34 3230 2c79  0,110,1750,420,y
-000096a0: 6573 2c34 2c73 7576 2f63 726f 7373 6f76  es,4,suv/crossov
-000096b0: 6572 2c35 2c32 3031 342c 3432 3933 302c  er,5,2014,42930,
-000096c0: 352c 3230 3132 2c6d 616e 7561 6c2c 3131  5,2012,manual,11
-000096d0: 2e37 2c36 2e32 2c31 3635 2c46 2c35 2e36  .7,6.2,165,F,5.6
-000096e0: 2c31 3831 2c37 2e34 2c34 2e35 332c 3231  ,181,7.4,4.53,21
-000096f0: 3030 2c31 3731 302c 3235 3035 2c37 352c  00,1710,2505,75,
-00009700: 3936 2c33 3335 2e30 3435 2c33 3537 2e39  96,335.045,357.9
-00009710: 3132 3632 3134 2c5b 332e 3735 2d20 312e  126214,[3.75- 1.
-00009720: 3931 2d20 312e 3138 2d20 302e 3834 2d20  91- 1.18- 0.84- 
-00009730: 302e 3635 2d20 302e 3534 5d2c 3136 3634  0.65- 0.54],1664
-00009740: 2e31 2c31 3733 392e 312c 3137 3634 2e31  .1,1739.1,1764.1
-00009750: 2c31 3730 302c 332e 3332 3334 2c4a 0d0a  ,1700,3.3234,J..
-00009760: 3930 3031 2c4a 2c31 3131 3639 2c79 6573  9001,J,11169,yes
-00009770: 2c79 6573 2c79 6573 2c79 6573 2c2c 6e6f  ,yes,yes,yes,,no
-00009780: 2c79 6573 2c79 6573 2c6e 6f2c 2c66 7565  ,yes,yes,no,,fue
-00009790: 6c20 656e 6769 6e65 2c70 6574 726f 6c2c  l engine,petrol,
-000097a0: 3238 352c 3533 302c 6672 6f6e 742b 7265  285,530,front+re
-000097b0: 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e39  ar,,,,,,,,,,,1.9
-000097c0: 3536 2c34 2e32 3637 2c32 2e34 2c31 2e37  56,4.267,2.4,1.7
-000097d0: 362c 2c35 3436 312c 7265 6775 6c61 722c  6,,5461,regular,
-000097e0: 382c 6f68 632c 6d75 6c74 6970 6f69 6e74  8,ohc,multipoint
-000097f0: 2069 6e6a 6563 7469 6f6e 2c39 362c 3630   injection,96,60
-00009800: 3030 2c32 3835 2c32 3830 302c 3533 302c  00,285,2800,530,
-00009810: 6e6f 2c34 2c73 7576 2f63 726f 7373 6f76  no,4,suv/crossov
-00009820: 6572 2c32 2c32 3031 342c 3139 3839 3030  er,2,2014,198900
-00009830: 2c34 2c32 3031 332c 6175 746f 6d61 7469  ,4,2013,automati
-00009840: 632c 352e 392c 3134 2e39 2c33 3438 2c47  c,5.9,14.9,348,G
-00009850: 2c31 312e 392c 3231 302c 3230 2c34 2e33  ,11.9,210,20,4.3
-00009860: 382c 3236 3030 2c32 3233 352c 3238 3530  8,2600,2235,2850
-00009870: 2c2c 3930 2e35 2c33 3532 2e36 322c 3337  ,,90.5,352.62,37
-00009880: 362e 3331 3036 3739 362c 5b34 2e33 382d  6.3106796,[4.38-
-00009890: 2032 2e38 362d 2031 2e39 322d 2031 2e33   2.86- 1.92- 1.3
-000098a0: 372d 2031 2e30 2d20 302e 3832 2d20 302e  7- 1.0- 0.82- 0.
-000098b0: 3733 5d2c 3231 3730 2e32 2c32 3234 352e  73],2170.2,2245.
-000098c0: 322c 3232 3730 2e32 2c32 3237 302c 332e  2,2270.2,2270,3.
-000098d0: 3434 3235 362c 4a0d 0a39 3535 312c 4a2c  44256,J..9551,J,
-000098e0: 3131 3739 362c 7965 732c 7965 732c 7965  11796,yes,yes,ye
-000098f0: 732c 7965 732c 2c6e 6f2c 7965 732c 7965  s,yes,,no,yes,ye
-00009900: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
-00009910: 6e65 2c70 6574 726f 6c2c 3432 332c 3735  ne,petrol,423,75
-00009920: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
-00009930: 2c2c 2c2c 2c2c 2c31 2e37 3534 2c34 2e38  ,,,,,,,1.754,4.8
-00009940: 382c 322e 3933 332c 312e 3938 352c 2c34  8,2.933,1.985,,4
-00009950: 3339 352c 7265 6775 6c61 722c 382c 646f  395,regular,8,do
-00009960: 6863 2c64 6972 6563 7420 696e 6a65 6374  hc,direct inject
-00009970: 696f 6e2c 3835 2c36 3030 302c 3432 332c  ion,85,6000,423,
-00009980: 3232 3030 2c37 3530 2c79 6573 2c34 2c73  2200,750,yes,4,s
-00009990: 7576 2f63 726f 7373 6f76 6572 2c35 2c61  uv/crossover,5,a
-000099a0: 7661 696c 6162 6c65 2c31 3634 3730 302c  vailable,164700,
-000099b0: 352d 4a75 6c2c 3230 3135 2c61 7574 6f6d  5-Jul,2015,autom
-000099c0: 6174 6963 2c34 2e32 2c31 312e 312c 3235  atic,4.2,11.1,25
-000099d0: 382c 472c 392c 3235 302c 3134 2e37 2c33  8,G,9,250,14.7,3
-000099e0: 2e31 352c 3137 3530 2c32 3235 302c 3239  .15,1750,2250,29
-000099f0: 3730 2c31 3030 2c38 382e 332c 3334 322e  70,100,88.3,342.
-00009a00: 3932 2c33 3537 2e32 3831 3535 3334 2c5b  92,357.2815534,[
-00009a10: 352e 302d 2033 2e32 2d20 322e 3134 2d20  5.0- 3.2- 2.14- 
-00009a20: 312e 3732 2d20 312e 3331 2d20 312e 302d  1.72- 1.31- 1.0-
-00009a30: 2030 2e38 322d 2030 2e36 345d 2c32 3139   0.82- 0.64],219
-00009a40: 322e 3632 352c 3232 3637 2e36 3235 2c32  2.625,2267.625,2
-00009a50: 3239 322e 3632 352c 3232 3730 2c33 2e34  292.625,2270,3.4
-00009a60: 3831 3639 2c4a 0d0a 3632 3232 2c4a 2c37  8169,J..6222,J,7
-00009a70: 3539 322c 7965 732c 7965 732c 7965 732c  592,yes,yes,yes,
-00009a80: 7965 732c 2c36 3330 2c6e 6f2c 7965 732c  yes,,630,no,yes,
-00009a90: 7965 732c 2c66 7565 6c20 656e 6769 6e65  yes,,fuel engine
-00009aa0: 2c64 6965 7365 6c2c 3139 302c 3536 302c  ,diesel,190,560,
-00009ab0: 6672 6f6e 742b 7265 6172 2c2c 2c2c 2c2c  front+rear,,,,,,
-00009ac0: 2c2c 2c2c 2c31 2e36 3631 2c34 2e36 3537  ,,,,,1.661,4.657
-00009ad0: 2c32 2e38 312c 312e 3838 312c 2c32 3939  ,2.81,1.881,,299
-00009ae0: 332c 7061 7274 6963 6c65 2066 696c 7465  3,particle filte
-00009af0: 722c 362c 646f 6863 2c63 6f6d 6d6f 6e20  r,6,dohc,common 
-00009b00: 7261 696c 2c36 372c 3430 3030 2c31 3930  rail,67,4000,190
-00009b10: 2c31 3530 302c 3536 302c 7965 732c 342c  ,1500,560,yes,4,
-00009b20: 7375 762f 6372 6f73 736f 7665 722c 352c  suv/crossover,5,
-00009b30: 6176 6169 6c61 626c 652c 3730 3838 362c  available,70886,
-00009b40: 352c 3230 3134 2c61 7574 6f6d 6174 6963  5,2014,automatic
-00009b50: 2c35 2e39 2c35 2e39 2c31 3536 2c45 2c35  ,5.9,5.9,156,E,5
-00009b60: 2e36 2c32 3332 2c36 2e35 2c32 2e38 312c  .6,232,6.5,2.81,
-00009b70: 3137 3030 2c31 3739 352c 3234 3130 2c31  1700,1795,2410,1
-00009b80: 3030 2c39 302c 3332 312e 322c 3334 302e  00,90,321.2,340.
-00009b90: 3637 3936 3131 372c 5b34 2e37 312d 2033  6796117,[4.71- 3
-00009ba0: 2e31 342d 2032 2e31 312d 2031 2e36 372d  .14- 2.11- 1.67-
-00009bb0: 2031 2e32 392d 2031 2e30 2d20 302e 3834   1.29- 1.0- 0.84
-00009bc0: 2d20 302e 3637 5d2c 3137 3439 2e37 3735  - 0.67],1749.775
-00009bd0: 2c31 3832 342e 3737 352c 3138 3439 2e37  ,1824.775,1849.7
-00009be0: 3735 2c31 3831 302c 332e 3132 3433 3431  75,1810,3.124341
-00009bf0: 2c4a 0d0a                                ,J..
+000084f0: 7661 696c 6162 6c65 2c33 3836 3435 2c30  vailable,38645,0
+00008500: 352d 4a75 6c2c 3230 3135 2c6d 616e 7561  5-Jul,2015,manua
+00008510: 6c2c 392e 382c 342e 392c 3132 392c 442c  l,9.8,4.9,129,D,
+00008520: 342e 322c 3230 382c 362e 312c 332e 3335  4.2,208,6.1,3.35
+00008530: 2c32 3030 302c 3136 3333 2c32 3431 302c  ,2000,1633,2410,
+00008540: 2c39 302e 342c 3330 332e 3635 2c33 3138  ,90.4,303.65,318
+00008550: 2e38 3334 3935 3135 2c5b 342e 3137 2d20  .8349515,[4.17- 
+00008560: 322e 3133 2d20 312e 3332 2d20 302e 3935  2.13- 1.32- 0.95
+00008570: 2d20 302e 3736 2d20 302e 3632 5d2c 3135  - 0.76- 0.62],15
+00008580: 3933 2e38 352c 3136 3638 2e38 352c 3136  93.85,1668.85,16
+00008590: 3933 2e38 352c 3137 3030 2c33 2e30 3636  93.85,1700,3.066
+000085a0: 372c 4d0d 0a37 3937 392c 4d2c 3935 3635  7,M..7979,M,9565
+000085b0: 2c79 6573 2c79 6573 2c79 6573 2c6e 6f2c  ,yes,yes,yes,no,
+000085c0: 2c6e 6f2c 3532 352c 7965 732c 6e6f 2c2c  ,no,525,yes,no,,
+000085d0: 6675 656c 2065 6e67 696e 652c 7065 7472  fuel engine,petr
+000085e0: 6f6c 2c38 382c 3136 302c 6672 6f6e 742c  ol,88,160,front,
+000085f0: 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3830 312c  ,,,,,,,,,,1.801,
+00008600: 342e 3338 2c32 2e37 3238 2c31 2e38 312c  4.38,2.728,1.81,
+00008610: 2c31 3539 382c 7265 6775 6c61 722c 342c  ,1598,regular,4,
+00008620: 6f68 632c 6d75 6c74 6970 6f69 6e74 2069  ohc,multipoint i
+00008630: 6e6a 6563 7469 6f6e 2c36 302c 3630 3030  njection,60,6000
+00008640: 2c38 382c 3432 3530 2c31 3630 2c6e 6f2c  ,88,4250,160,no,
+00008650: 342c 6d70 762c 352c 6176 6169 6c61 626c  4,mpv,5,availabl
+00008660: 652c 3238 3135 302c 352c 3230 3133 2c6d  e,28150,5,2013,m
+00008670: 616e 7561 6c2c 3132 2c37 2e33 2c31 3639  anual,12,7.3,169
+00008680: 2c45 2c36 2c31 3737 2c39 2e36 2c35 2e30  ,E,6,177,9.6,5.0
+00008690: 372c 3337 3030 2c31 3239 352c 3230 3030  7,3700,1295,2000
+000086a0: 2c31 3030 2c38 352e 352c 3239 342e 3433  ,100,85.5,294.43
+000086b0: 352c 3331 342e 3332 3033 3838 332c 5b33  5,314.3203883,[3
+000086c0: 2e34 352d 2031 2e38 372d 2031 2e32 392d  .45- 1.87- 1.29-
+000086d0: 2030 2e39 352d 2030 2e37 345d 2c31 3235   0.95- 0.74],125
+000086e0: 342e 352c 3133 3239 2e35 2c31 3335 342e  4.5,1329.5,1354.
+000086f0: 352c 3133 3630 2c33 2e32 3539 3831 2c4d  5,1360,3.25981,M
+00008700: 0d0a 3232 3539 312c 4a2c 3331 3230 352c  ..22591,J,31205,
+00008710: 7965 732c 7965 732c 7965 732c 6e6f 2c2c  yes,yes,yes,no,,
+00008720: 3435 302c 7965 732c 7965 732c 6e6f 2c2c  450,yes,yes,no,,
+00008730: 6675 656c 2065 6e67 696e 652c 6469 6573  fuel engine,dies
+00008740: 656c 2c31 3330 2c33 3530 2c66 726f 6e74  el,130,350,front
+00008750: 2b72 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c  +rear,,,,,,,,,,,
+00008760: 312e 3730 332c 342e 3432 362c 322e 3630  1.703,4.426,2.60
+00008770: 342c 312e 3830 392c 2c31 3936 382c 7061  4,1.809,,1968,pa
+00008780: 7274 6963 6c65 2066 696c 7465 722c 342c  rticle filter,4,
+00008790: 646f 6863 2c63 6f6d 6d6f 6e20 7261 696c  dohc,common rail
+000087a0: 2c36 342c 3432 3030 2c31 3330 2c31 3735  ,64,4200,130,175
+000087b0: 302c 3335 302c 7965 732c 342c 7375 762f  0,350,yes,4,suv/
+000087c0: 6372 6f73 736f 7665 722c 352c 6176 6169  crossover,5,avai
+000087d0: 6c61 626c 652c 3439 3939 302c 352c 3230  lable,49990,5,20
+000087e0: 3133 2c6d 616e 7561 6c2c 382e 352c 352e  13,manual,8.5,5.
+000087f0: 382c 3135 312c 472c 352e 322c 3230 322c  8,151,G,5.2,202,
+00008800: 362e 372c 332e 3035 2c32 3135 302c 3135  6.7,3.05,2150,15
+00008810: 3738 2c32 3234 302c 3735 2c39 352e 352c  78,2240,75,95.5,
+00008820: 3331 362e 3731 352c 3333 352e 3039 3730  316.715,335.0970
+00008830: 3837 342c 5b33 2e39 322d 2032 2e30 352d  874,[3.92- 2.05-
+00008840: 2031 2e37 352d 2031 2e32 332d 2030 2e39   1.75- 1.23- 0.9
+00008850: 342d 2030 2e37 375d 2c31 3533 342e 382c  4- 0.77],1534.8,
+00008860: 3136 3039 2e38 2c31 3633 342e 382c 3135  1609.8,1634.8,15
+00008870: 3930 2c33 2e30 3830 3732 372c 4a0d 0a33  90,3.080727,J..3
+00008880: 3432 3032 2c4a 2c34 3836 3532 2c79 6573  4202,J,48652,yes
+00008890: 2c79 6573 2c79 6573 2c6e 6f2c 2c79 6573  ,yes,yes,no,,yes
+000088a0: 2c79 6573 2c79 6573 2c6e 6f2c 2c66 7565  ,yes,yes,no,,fue
+000088b0: 6c20 656e 6769 6e65 2c70 6574 726f 6c2c  l engine,petrol,
+000088c0: 3838 2c31 3930 2c66 726f 6e74 2c2c 2c2c  88,190,front,,,,
+000088d0: 2c2c 2c2c 2c2c 2c31 2e35 3636 2c34 2e31  ,,,,,,,1.566,4.1
+000088e0: 3232 2c32 2e36 3036 2c31 2e37 3738 2c2c  22,2.606,1.778,,
+000088f0: 3131 3936 2c72 6567 756c 6172 2c34 2c64  1196,regular,4,d
+00008900: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
+00008910: 7469 6f6e 2c34 352c 3439 3030 2c38 382c  tion,45,4900,88,
+00008920: 3230 3030 2c31 3930 2c79 6573 2c34 2c73  2000,190,yes,4,s
+00008930: 7576 2f63 726f 7373 6f76 6572 2c35 2c61  uv/crossover,5,a
+00008940: 7661 696c 6162 6c65 2c32 3531 3930 2c35  vailable,25190,5
+00008950: 2c32 3031 352c 6175 746f 6d61 7469 632c  ,2015,automatic,
+00008960: 3130 2e39 2c35 2e34 2c31 3235 2c42 2c34  10.9,5.4,125,B,4
+00008970: 2e37 2c31 3932 2c36 2e36 2c33 2e39 352c  .7,192,6.6,3.95,
+00008980: 3236 3530 2c31 3135 352c 3137 3236 2c2c  2650,1155,1726,,
+00008990: 3733 2e31 2c33 3033 2e38 3435 2c33 3139  73.1,303.845,319
+000089a0: 2e30 3737 3636 3939 2c5b 332e 3932 2d20  .0776699,[3.92- 
+000089b0: 322e 3433 2d20 312e 3434 2d20 312e 3032  2.43- 1.44- 1.02
+000089c0: 2d20 302e 3837 2d20 302e 375d 2c31 3132  - 0.87- 0.7],112
+000089d0: 342e 3632 352c 3131 3939 2e36 3235 2c31  4.625,1199.625,1
+000089e0: 3232 342e 3632 352c 3132 3530 2c32 2e37  224.625,1250,2.7
+000089f0: 3834 3334 382c 4a0d 0a34 3031 3730 2c4a  84348,J..40170,J
+00008a00: 2c35 3731 3438 2c79 6573 2c79 6573 2c79  ,57148,yes,yes,y
+00008a10: 6573 2c79 6573 2c2c 7965 732c 7965 732c  es,yes,,yes,yes,
+00008a20: 7965 732c 7965 732c 2c66 7565 6c20 656e  yes,yes,,fuel en
+00008a30: 6769 6e65 2c70 6574 726f 6c2c 3835 2c31  gine,petrol,85,1
+00008a40: 3930 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  90,front,,,,,,,,
+00008a50: 2c2c 2c31 2e35 392c 342e 3337 372c 322e  ,,,1.59,4.377,2.
+00008a60: 3634 362c 312e 3830 362c 2c31 3139 372c  646,1.806,,1197,
+00008a70: 7265 6775 6c61 722c 342c 646f 6863 2c64  regular,4,dohc,d
+00008a80: 6972 6563 7420 696e 6a65 6374 696f 6e2c  irect injection,
+00008a90: 3535 2c34 3530 302c 3835 2c32 3030 302c  55,4500,85,2000,
+00008aa0: 3139 302c 7965 732c 342c 7375 762f 6372  190,yes,4,suv/cr
+00008ab0: 6f73 736f 7665 722c 352c 3230 3135 2c33  ossover,5,2015,3
+00008ac0: 3031 3930 2c35 2c32 3031 342c 6d61 6e75  0190,5,2014,manu
+00008ad0: 616c 2c31 312e 332c 352e 382c 3132 392c  al,11.3,5.8,129,
+00008ae0: 422c 342e 392c 3138 332c 362e 392c 342e  B,4.9,183,6.9,4.
+00008af0: 3231 2c32 3530 302c 3132 3530 2c31 3836  21,2500,1250,186
+00008b00: 302c 3735 2c37 332e 312c 3332 302e 3237  0,75,73.1,320.27
+00008b10: 352c 3333 322e 3537 3238 3135 352c 5b33  5,332.5728155,[3
+00008b20: 2e37 332d 2031 2e39 352d 2031 2e33 322d  .73- 1.95- 1.32-
+00008b30: 2030 2e39 382d 2030 2e37 362d 2030 2e36   0.98- 0.76- 0.6
+00008b40: 345d 2c31 3231 322e 3837 352c 3132 3837  4],1212.875,1287
+00008b50: 2e38 3735 2c31 3331 322e 3837 352c 3132  .875,1312.875,12
+00008b60: 3530 2c32 2e38 3731 3534 2c4a 0d0a 3434  50,2.87154,J..44
+00008b70: 3539 392c 4a2c 3633 3438 322c 7965 732c  599,J,63482,yes,
+00008b80: 7965 732c 7965 732c 7965 732c 2c79 6573  yes,yes,yes,,yes
+00008b90: 2c79 6573 2c79 6573 2c79 6573 2c2c 6675  ,yes,yes,yes,,fu
+00008ba0: 656c 2065 6e67 696e 652c 6469 6573 656c  el engine,diesel
+00008bb0: 2c39 362c 3332 302c 6672 6f6e 742c 2c2c  ,96,320,front,,,
+00008bc0: 2c2c 2c2c 2c2c 2c2c 312e 3539 2c34 2e33  ,,,,,,,,1.59,4.3
+00008bd0: 3737 2c32 2e36 3436 2c31 2e38 3036 2c2c  77,2.646,1.806,,
+00008be0: 3135 3938 2c70 6172 7469 636c 6520 6669  1598,particle fi
+00008bf0: 6c74 6572 2c34 2c64 6f68 632c 636f 6d6d  lter,4,dohc,comm
+00008c00: 6f6e 2072 6169 6c2c 3535 2c34 3030 302c  on rail,55,4000,
+00008c10: 3936 2c31 3735 302c 3332 302c 7965 732c  96,1750,320,yes,
+00008c20: 342c 7375 762f 6372 6f73 736f 7665 722c  4,suv/crossover,
+00008c30: 352c 6176 6169 6c61 626c 652c 3335 3530  5,available,3550
+00008c40: 302c 352c 3230 3134 2c6d 616e 7561 6c2c  0,5,2014,manual,
+00008c50: 3130 2e35 2c34 2e34 2c31 3135 2c44 2c33  10.5,4.4,115,D,3
+00008c60: 2e39 2c31 3930 2c35 2e32 2c34 2e31 332c  .9,190,5.2,4.13,
+00008c70: 3233 3030 2c31 3334 302c 3139 3630 2c37  2300,1340,1960,7
+00008c80: 352c 3739 2e35 2c33 3230 2e32 3735 2c33  5,79.5,320.275,3
+00008c90: 3332 2e35 3732 3831 3535 2c5b 332e 3733  32.5728155,[3.73
+00008ca0: 2d20 322e 3034 2d20 312e 3332 2d20 302e  - 2.04- 1.32- 0.
+00008cb0: 3935 2d20 302e 3732 2d20 302e 365d 2c31  95- 0.72- 0.6],1
+00008cc0: 3330 322e 3837 352c 3133 3737 2e38 3735  302.875,1377.875
+00008cd0: 2c31 3430 322e 3837 352c 3133 3630 2c32  ,1402.875,1360,2
+00008ce0: 2e38 3731 3534 2c4a 0d0a 3533 3538 2c4a  .87154,J..5358,J
+00008cf0: 2c36 3632 392c 7965 732c 7965 732c 7965  ,6629,yes,yes,ye
+00008d00: 732c 7965 732c 2c79 6573 2c79 6573 2c79  s,yes,,yes,yes,y
+00008d10: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
+00008d20: 696e 652c 7065 7472 6f6c 2c31 3632 2c33  ine,petrol,162,3
+00008d30: 3530 2c66 726f 6e74 2b72 6561 722c 2c2c  50,front+rear,,,
+00008d40: 2c2c 2c2c 2c2c 2c2c 312e 3630 382c 342e  ,,,,,,,,1.608,4.
+00008d50: 3338 382c 322e 3630 332c 312e 3833 312c  388,2.603,1.831,
+00008d60: 2c31 3938 342c 7265 6775 6c61 722c 342c  ,1984,regular,4,
+00008d70: 646f 6863 2c64 6972 6563 7420 696e 6a65  dohc,direct inje
+00008d80: 6374 696f 6e2c 3634 2c34 3530 302c 3136  ction,64,4500,16
+00008d90: 322c 3135 3030 2c33 3530 2c79 6573 2c34  2,1500,350,yes,4
+00008da0: 2c73 7576 2f63 726f 7373 6f76 6572 2c35  ,suv/crossover,5
+00008db0: 2c61 7661 696c 6162 6c65 2c35 3237 3030  ,available,52700
+00008dc0: 2c35 2c32 3031 352c 6175 746f 6d61 7469  ,5,2015,automati
+00008dd0: 632c 362e 342c 362e 372c 3135 342c 442c  c,6.4,6.7,154,D,
+00008de0: 352e 392c 3233 332c 382e 312c 332e 3934  5.9,233,8.1,3.94
+00008df0: 2c32 3330 302c 3135 3430 2c32 3136 352c  ,2300,1540,2165,
+00008e00: 3735 2c39 322e 382c 3331 362e 3731 352c  75,92.8,316.715,
+00008e10: 3333 352e 3039 3730 3837 342c 5b33 2e35  335.0970874,[3.5
+00008e20: 362d 2032 2e35 332d 2031 2e36 382d 2031  6- 2.53- 1.68- 1
+00008e30: 2e30 322d 2030 2e37 392d 2030 2e37 362d  .02- 0.79- 0.76-
+00008e40: 2030 2e36 345d 2c31 3439 362e 382c 3135   0.64],1496.8,15
+00008e50: 3731 2e38 2c31 3539 362e 382c 3135 3930  71.8,1596.8,1590
+00008e60: 2c32 2e39 3434 3234 382c 4a0d 0a35 3333  ,2.944248,J..533
+00008e70: 382c 4a2c 3636 3039 2c79 6573 2c79 6573  8,J,6609,yes,yes
+00008e80: 2c79 6573 2c79 6573 2c2c 7965 732c 7965  ,yes,yes,,yes,ye
+00008e90: 732c 7965 732c 7965 732c 2c66 7565 6c20  s,yes,yes,,fuel 
+00008ea0: 656e 6769 6e65 2c64 6965 7365 6c2c 3133  engine,diesel,13
+00008eb0: 352c 3338 302c 6672 6f6e 742b 7265 6172  5,380,front+rear
+00008ec0: 2c2c 2c2c 2c2c 2c2c 2c2c 2c31 2e36 3038  ,,,,,,,,,,,1.608
+00008ed0: 2c34 2e33 3838 2c32 2e36 3033 2c31 2e38  ,4.388,2.603,1.8
+00008ee0: 3331 2c2c 3139 3638 2c70 6172 7469 636c  31,,1968,particl
+00008ef0: 6520 6669 6c74 6572 2c34 2c64 6f68 632c  e filter,4,dohc,
+00008f00: 636f 6d6d 6f6e 2072 6169 6c2c 3634 2c33  common rail,64,3
+00008f10: 3530 302c 3133 352c 3138 3030 2c33 3830  500,135,1800,380
+00008f20: 2c79 6573 2c34 2c73 7576 2f63 726f 7373  ,yes,4,suv/cross
+00008f30: 6f76 6572 2c35 2c61 7661 696c 6162 6c65  over,5,available
+00008f40: 2c35 3135 3630 2c35 2c32 3031 352c 6d61  ,51560,5,2015,ma
+00008f50: 6e75 616c 2c37 2e39 2c35 2e32 2c31 3337  nual,7.9,5.2,137
+00008f60: 2c46 2c34 2e35 2c32 3139 2c36 2e35 2c33  ,F,4.5,219,6.5,3
+00008f70: 2e33 372c 3234 3030 2c31 3538 302c 3232  .37,2400,1580,22
+00008f80: 3035 2c37 352c 3935 2e35 2c33 3136 2e37  05,75,95.5,316.7
+00008f90: 3135 2c33 3335 2e30 3937 3038 3734 2c5b  15,335.0970874,[
+00008fa0: 332e 3932 2d20 322e 3035 2d20 312e 3735  3.92- 2.05- 1.75
+00008fb0: 2d20 312e 3233 2d20 302e 3934 2d20 302e  - 1.23- 0.94- 0.
+00008fc0: 3737 5d2c 3135 3336 2e38 2c31 3631 312e  77],1536.8,1611.
+00008fd0: 382c 3136 3336 2e38 2c31 3539 302c 322e  8,1636.8,1590,2.
+00008fe0: 3934 3432 3438 2c4a 0d0a 3334 3031 352c  944248,J..34015,
+00008ff0: 4a2c 3438 3435 302c 7965 732c 7965 732c  J,48450,yes,yes,
+00009000: 7965 732c 7965 732c 2c6e 6f2c 7965 732c  yes,yes,,no,yes,
+00009010: 7965 732c 7965 732c 2c66 7565 6c20 656e  yes,yes,,fuel en
+00009020: 6769 6e65 2c64 6965 7365 6c2c 3838 2c33  gine,diesel,88,3
+00009030: 3030 2c66 726f 6e74 2c2c 2c2c 2c2c 2c2c  00,front,,,,,,,,
+00009040: 2c2c 2c31 2e35 3536 2c34 2e31 3539 2c32  ,,,1.556,4.159,2
+00009050: 2e35 3338 2c31 2e37 3339 2c2c 3135 3630  .538,1.739,,1560
+00009060: 2c72 6567 756c 6172 2c34 2c64 6f68 632c  ,regular,4,dohc,
+00009070: 636f 6d6d 6f6e 2072 6169 6c2c 3530 2c33  common rail,50,3
+00009080: 3530 302c 3838 2c31 3735 302c 3330 302c  500,88,1750,300,
+00009090: 7965 732c 342c 7375 762f 6372 6f73 736f  yes,4,suv/crosso
+000090a0: 7665 722c 352c 6176 6169 6c61 626c 652c  ver,5,available,
+000090b0: 3236 3735 302c 352c 3230 3135 2c6d 616e  26750,5,2015,man
+000090c0: 7561 6c2c 3130 2e34 2c33 2e37 2c39 362c  ual,10.4,3.7,96,
+000090d0: 432c 332e 332c 3139 322c 342e 332c 332e  C,3.3,192,4.3,3.
+000090e0: 3734 2c32 3235 302c 3131 3735 2c31 3732  74,2250,1175,172
+000090f0: 362c 2c38 382e 332c 3239 342e 3436 2c33  6,,88.3,294.46,3
+00009100: 3130 2e38 3733 3738 3634 2c5b 332e 3835  10.8737864,[3.85
+00009110: 2d20 322e 3039 2d20 312e 3339 2d20 302e  - 2.09- 1.39- 0.
+00009120: 3939 2d20 302e 3733 2d20 302e 3631 5d2c  99- 0.73- 0.61],
+00009130: 3131 3431 2e32 352c 3132 3136 2e32 352c  1141.25,1216.25,
+00009140: 3132 3431 2e32 352c 3132 3530 2c32 2e37  1241.25,1250,2.7
+00009150: 3035 3838 342c 4a0d 0a39 3837 322c 4a2c  05884,J..9872,J,
+00009160: 3132 3237 372c 7965 732c 7965 732c 7965  12277,yes,yes,ye
+00009170: 732c 7965 732c 2c79 6573 2c79 6573 2c79  s,yes,,yes,yes,y
+00009180: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
+00009190: 696e 652c 7065 7472 6f6c 2c33 3735 2c36  ine,petrol,375,6
+000091a0: 3235 2c66 726f 6e74 2b72 6561 722c 2c2c  25,front+rear,,,
+000091b0: 2c2c 2c2c 2c2c 2c2c 312e 3833 352c 342e  ,,,,,,,,1.835,4.
+000091c0: 3939 392c 322e 3932 322c 312e 3938 332c  999,2.922,1.983,
+000091d0: 2c35 3030 302c 7265 6775 6c61 722c 382c  ,5000,regular,8,
+000091e0: 646f 6863 2c6d 756c 7469 706f 696e 7420  dohc,multipoint 
+000091f0: 696e 6a65 6374 696f 6e2c 3130 352c 3630  injection,105,60
+00009200: 3030 2c33 3735 2c32 3530 302c 3632 352c  00,375,2500,625,
+00009210: 7965 732c 342c 7375 762f 6372 6f73 736f  yes,4,suv/crosso
+00009220: 7665 722c 352c 6176 6169 6c61 626c 652c  ver,5,available,
+00009230: 3233 3537 3030 2c35 2c32 3031 342c 6175  235700,5,2014,au
+00009240: 746f 6d61 7469 632c 352e 342c 3132 2e38  tomatic,5.4,12.8
+00009250: 2c32 3939 2c47 2c39 2e37 2c32 3235 2c31  ,299,G,9.7,225,1
+00009260: 382e 332c 332e 3331 2c31 3830 302c 3233  8.3,3.31,1800,23
+00009270: 3330 2c33 3135 302c 3130 302c 3933 2c33  30,3150,100,93,3
+00009280: 3633 2e33 3935 2c33 3832 2e37 3636 3939  63.395,382.76699
+00009290: 3033 2c5b 342e 372d 2033 2e31 332d 2032  03,[4.7- 3.13- 2
+000092a0: 2e31 2d20 312e 3637 2d20 312e 3239 2d20  .1- 1.67- 1.29- 
+000092b0: 312e 302d 2030 2e38 342d 2030 2e36 375d  1.0- 0.84- 0.67]
+000092c0: 2c32 3235 392e 3132 352c 3233 3334 2e31  ,2259.125,2334.1
+000092d0: 3235 2c32 3335 392e 3132 352c 3232 3730  25,2359.125,2270
+000092e0: 2c33 2e36 3338 3830 352c 4a0d 0a39 3835  ,3.638805,J..985
+000092f0: 362c 4a2c 3132 3236 312c 7965 732c 7965  6,J,12261,yes,ye
+00009300: 732c 7965 732c 7965 732c 2c79 6573 2c79  s,yes,yes,,yes,y
+00009310: 6573 2c79 6573 2c79 6573 2c2c 6675 656c  es,yes,yes,,fuel
+00009320: 2065 6e67 696e 652c 6469 6573 656c 2c31   engine,diesel,1
+00009330: 3930 2c36 3030 2c66 726f 6e74 2b72 6561  90,600,front+rea
+00009340: 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e 3834  r,,,,,,,,,,,1.84
+00009350: 2c35 2e31 3939 2c33 2e31 322c 312e 3938  ,5.199,3.12,1.98
+00009360: 332c 2c32 3939 332c 7061 7274 6963 6c65  3,,2993,particle
+00009370: 2066 696c 7465 722c 362c 646f 6863 2c63   filter,6,dohc,c
+00009380: 6f6d 6d6f 6e20 7261 696c 2c38 352c 3430  ommon rail,85,40
+00009390: 3030 2c31 3930 2c32 3030 302c 3630 302c  00,190,2000,600,
+000093a0: 7965 732c 342c 7375 762f 6372 6f73 736f  yes,4,suv/crosso
+000093b0: 7665 722c 352c 6176 6169 6c61 626c 652c  ver,5,available,
+000093c0: 3134 3835 3030 2c35 2c32 3031 342c 6175  148500,5,2014,au
+000093d0: 746f 6d61 7469 632c 372e 392c 362e 392c  tomatic,7.9,6.9,
+000093e0: 3138 322c 432c 362e 332c 3231 302c 372e  182,C,6.3,210,7.
+000093f0: 382c 332e 3231 2c31 3735 302c 3233 3031  8,3.21,1750,2301
+00009400: 2c33 3035 302c 3130 302c 3930 2c33 3633  ,3050,100,90,363
+00009410: 2e33 3935 2c33 3832 2e37 3636 3939 3033  .395,382.7669903
+00009420: 2c5b 342e 372d 2033 2e31 332d 2032 2e31  ,[4.7- 3.13- 2.1
+00009430: 2d20 312e 3637 2d20 312e 3239 2d20 312e  - 1.67- 1.29- 1.
+00009440: 302d 2030 2e38 342d 2030 2e36 375d 2c32  0- 0.84- 0.67],2
+00009450: 3234 332e 3632 352c 3233 3138 2e36 3235  243.625,2318.625
+00009460: 2c32 3334 332e 3632 352c 3232 3730 2c33  ,2343.625,2270,3
+00009470: 2e36 3438 3732 2c4a 0d0a 3634 3436 2c4a  .64872,J..6446,J
+00009480: 2c37 3932 392c 7965 732c 7965 732c 7965  ,7929,yes,yes,ye
+00009490: 732c 7965 732c 2c36 3630 2c79 6573 2c79  s,yes,,660,yes,y
+000094a0: 6573 2c6e 6f2c 2c66 7565 6c20 656e 6769  es,no,,fuel engi
+000094b0: 6e65 2c70 6574 726f 6c2c 3137 372c 3334  ne,petrol,177,34
+000094c0: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
+000094d0: 2c2c 2c2c 2c2c 2c31 2e37 3234 2c34 2e35  ,,,,,,,1.724,4.5
+000094e0: 3939 2c32 2e37 3431 2c31 2e38 3935 2c2c  99,2.741,1.895,,
+000094f0: 3139 3939 2c72 6567 756c 6172 2c34 2c64  1999,regular,4,d
+00009500: 6f68 632c 6d75 6c74 6970 6f69 6e74 2069  ohc,multipoint i
+00009510: 6e6a 6563 7469 6f6e 2c37 302c 3535 3030  njection,70,5500
+00009520: 2c31 3737 2c31 3735 302c 3334 302c 7965  ,177,1750,340,ye
+00009530: 732c 342c 7375 762f 6372 6f73 736f 7665  s,4,suv/crossove
+00009540: 722c 352c 6176 6169 6c61 626c 652c 3733  r,5,available,73
+00009550: 3230 302c 352c 3230 3134 2c61 7574 6f6d  200,5,2014,autom
+00009560: 6174 6963 2c38 2e32 2c38 2e32 2c31 3931  atic,8.2,8.2,191
+00009570: 2c45 2c2c 3139 392c 2c33 2e37 352c 2c31  ,E,,199,,3.75,,1
+00009580: 3734 342c 3235 3035 2c37 352c 3833 2e31  744,2505,75,83.1
+00009590: 2c33 3432 2e31 3135 2c33 3539 2e37 3537  ,342.115,359.757
+000095a0: 3238 3136 2c5b 342e 3135 2d20 322e 3337  2816,[4.15- 2.37
+000095b0: 2d20 312e 3536 2d20 312e 3136 2d20 302e  - 1.56- 1.16- 0.
+000095c0: 3836 2d20 302e 3639 5d2c 3136 3936 2e37  86- 0.69],1696.7
+000095d0: 352c 3137 3731 2e37 352c 3137 3936 2e37  5,1771.75,1796.7
+000095e0: 352c 3138 3130 2c33 2e32 3636 3938 2c4a  5,1810,3.26698,J
+000095f0: 0d0a 3838 3636 2c4a 2c31 3130 3133 2c79  ..8866,J,11013,y
+00009600: 6573 2c79 6573 2c34 3430 2c6e 6f2c 2c6e  es,yes,440,no,,n
+00009610: 6f2c 3431 302c 7965 732c 7965 732c 2c66  o,410,yes,yes,,f
+00009620: 7565 6c20 656e 6769 6e65 2c64 6965 7365  uel engine,diese
+00009630: 6c2c 3131 302c 3432 302c 6672 6f6e 742b  l,110,420,front+
+00009640: 7265 6172 2c2c 2c2c 2c2c 2c2c 2c2c 2c31  rear,,,,,,,,,,,1
+00009650: 2e37 342c 342e 352c 322e 3636 2c31 2e39  .74,4.5,2.66,1.9
+00009660: 312c 2c32 3137 392c 7061 7274 6963 6c65  1,,2179,particle
+00009670: 2066 696c 7465 722c 342c 646f 6863 2c63   filter,4,dohc,c
+00009680: 6f6d 6d6f 6e20 7261 696c 2c36 382c 3430  ommon rail,68,40
+00009690: 3030 2c31 3130 2c31 3735 302c 3432 302c  00,110,1750,420,
+000096a0: 7965 732c 342c 7375 762f 6372 6f73 736f  yes,4,suv/crosso
+000096b0: 7665 722c 352c 3230 3134 2c34 3239 3330  ver,5,2014,42930
+000096c0: 2c35 2c32 3031 322c 6d61 6e75 616c 2c31  ,5,2012,manual,1
+000096d0: 312e 372c 362e 322c 3136 352c 462c 352e  1.7,6.2,165,F,5.
+000096e0: 362c 3138 312c 372e 342c 342e 3533 2c32  6,181,7.4,4.53,2
+000096f0: 3130 302c 3137 3130 2c32 3530 352c 3735  100,1710,2505,75
+00009700: 2c39 362c 3333 352e 3034 352c 3335 372e  ,96,335.045,357.
+00009710: 3931 3236 3231 342c 5b33 2e37 352d 2031  9126214,[3.75- 1
+00009720: 2e39 312d 2031 2e31 382d 2030 2e38 342d  .91- 1.18- 0.84-
+00009730: 2030 2e36 352d 2030 2e35 345d 2c31 3636   0.65- 0.54],166
+00009740: 342e 312c 3137 3339 2e31 2c31 3736 342e  4.1,1739.1,1764.
+00009750: 312c 3137 3030 2c33 2e33 3233 342c 4a0d  1,1700,3.3234,J.
+00009760: 0a39 3030 312c 4a2c 3131 3136 392c 7965  .9001,J,11169,ye
+00009770: 732c 7965 732c 7965 732c 7965 732c 2c6e  s,yes,yes,yes,,n
+00009780: 6f2c 7965 732c 7965 732c 6e6f 2c2c 6675  o,yes,yes,no,,fu
+00009790: 656c 2065 6e67 696e 652c 7065 7472 6f6c  el engine,petrol
+000097a0: 2c32 3835 2c35 3330 2c66 726f 6e74 2b72  ,285,530,front+r
+000097b0: 6561 722c 2c2c 2c2c 2c2c 2c2c 2c2c 312e  ear,,,,,,,,,,,1.
+000097c0: 3935 362c 342e 3236 372c 322e 342c 312e  956,4.267,2.4,1.
+000097d0: 3736 2c2c 3534 3631 2c72 6567 756c 6172  76,,5461,regular
+000097e0: 2c38 2c6f 6863 2c6d 756c 7469 706f 696e  ,8,ohc,multipoin
+000097f0: 7420 696e 6a65 6374 696f 6e2c 3936 2c36  t injection,96,6
+00009800: 3030 302c 3238 352c 3238 3030 2c35 3330  000,285,2800,530
+00009810: 2c6e 6f2c 342c 7375 762f 6372 6f73 736f  ,no,4,suv/crosso
+00009820: 7665 722c 322c 3230 3134 2c31 3938 3930  ver,2,2014,19890
+00009830: 302c 342c 3230 3133 2c61 7574 6f6d 6174  0,4,2013,automat
+00009840: 6963 2c35 2e39 2c31 342e 392c 3334 382c  ic,5.9,14.9,348,
+00009850: 472c 3131 2e39 2c32 3130 2c32 302c 342e  G,11.9,210,20,4.
+00009860: 3338 2c32 3630 302c 3232 3335 2c32 3835  38,2600,2235,285
+00009870: 302c 2c39 302e 352c 3335 322e 3632 2c33  0,,90.5,352.62,3
+00009880: 3736 2e33 3130 3637 3936 2c5b 342e 3338  76.3106796,[4.38
+00009890: 2d20 322e 3836 2d20 312e 3932 2d20 312e  - 2.86- 1.92- 1.
+000098a0: 3337 2d20 312e 302d 2030 2e38 322d 2030  37- 1.0- 0.82- 0
+000098b0: 2e37 335d 2c32 3137 302e 322c 3232 3435  .73],2170.2,2245
+000098c0: 2e32 2c32 3237 302e 322c 3232 3730 2c33  .2,2270.2,2270,3
+000098d0: 2e34 3432 3536 2c4a 0d0a 3935 3531 2c4a  .44256,J..9551,J
+000098e0: 2c31 3137 3936 2c79 6573 2c79 6573 2c79  ,11796,yes,yes,y
+000098f0: 6573 2c79 6573 2c2c 6e6f 2c79 6573 2c79  es,yes,,no,yes,y
+00009900: 6573 2c79 6573 2c2c 6675 656c 2065 6e67  es,yes,,fuel eng
+00009910: 696e 652c 7065 7472 6f6c 2c34 3233 2c37  ine,petrol,423,7
+00009920: 3530 2c66 726f 6e74 2b72 6561 722c 2c2c  50,front+rear,,,
+00009930: 2c2c 2c2c 2c2c 2c2c 312e 3735 342c 342e  ,,,,,,,,1.754,4.
+00009940: 3838 2c32 2e39 3333 2c31 2e39 3835 2c2c  88,2.933,1.985,,
+00009950: 3433 3935 2c72 6567 756c 6172 2c38 2c64  4395,regular,8,d
+00009960: 6f68 632c 6469 7265 6374 2069 6e6a 6563  ohc,direct injec
+00009970: 7469 6f6e 2c38 352c 3630 3030 2c34 3233  tion,85,6000,423
+00009980: 2c32 3230 302c 3735 302c 7965 732c 342c  ,2200,750,yes,4,
+00009990: 7375 762f 6372 6f73 736f 7665 722c 352c  suv/crossover,5,
+000099a0: 6176 6169 6c61 626c 652c 3136 3437 3030  available,164700
+000099b0: 2c30 352d 4a75 6c2c 3230 3135 2c61 7574  ,05-Jul,2015,aut
+000099c0: 6f6d 6174 6963 2c34 2e32 2c31 312e 312c  omatic,4.2,11.1,
+000099d0: 3235 382c 472c 392c 3235 302c 3134 2e37  258,G,9,250,14.7
+000099e0: 2c33 2e31 352c 3137 3530 2c32 3235 302c  ,3.15,1750,2250,
+000099f0: 3239 3730 2c31 3030 2c38 382e 332c 3334  2970,100,88.3,34
+00009a00: 322e 3932 2c33 3537 2e32 3831 3535 3334  2.92,357.2815534
+00009a10: 2c5b 352e 302d 2033 2e32 2d20 322e 3134  ,[5.0- 3.2- 2.14
+00009a20: 2d20 312e 3732 2d20 312e 3331 2d20 312e  - 1.72- 1.31- 1.
+00009a30: 302d 2030 2e38 322d 2030 2e36 345d 2c32  0- 0.82- 0.64],2
+00009a40: 3139 322e 3632 352c 3232 3637 2e36 3235  192.625,2267.625
+00009a50: 2c32 3239 322e 3632 352c 3232 3730 2c33  ,2292.625,2270,3
+00009a60: 2e34 3831 3639 2c4a 0d0a 3632 3232 2c4a  .48169,J..6222,J
+00009a70: 2c37 3539 322c 7965 732c 7965 732c 7965  ,7592,yes,yes,ye
+00009a80: 732c 7965 732c 2c36 3330 2c6e 6f2c 7965  s,yes,,630,no,ye
+00009a90: 732c 7965 732c 2c66 7565 6c20 656e 6769  s,yes,,fuel engi
+00009aa0: 6e65 2c64 6965 7365 6c2c 3139 302c 3536  ne,diesel,190,56
+00009ab0: 302c 6672 6f6e 742b 7265 6172 2c2c 2c2c  0,front+rear,,,,
+00009ac0: 2c2c 2c2c 2c2c 2c31 2e36 3631 2c34 2e36  ,,,,,,,1.661,4.6
+00009ad0: 3537 2c32 2e38 312c 312e 3838 312c 2c32  57,2.81,1.881,,2
+00009ae0: 3939 332c 7061 7274 6963 6c65 2066 696c  993,particle fil
+00009af0: 7465 722c 362c 646f 6863 2c63 6f6d 6d6f  ter,6,dohc,commo
+00009b00: 6e20 7261 696c 2c36 372c 3430 3030 2c31  n rail,67,4000,1
+00009b10: 3930 2c31 3530 302c 3536 302c 7965 732c  90,1500,560,yes,
+00009b20: 342c 7375 762f 6372 6f73 736f 7665 722c  4,suv/crossover,
+00009b30: 352c 6176 6169 6c61 626c 652c 3730 3838  5,available,7088
+00009b40: 362c 352c 3230 3134 2c61 7574 6f6d 6174  6,5,2014,automat
+00009b50: 6963 2c35 2e39 2c35 2e39 2c31 3536 2c45  ic,5.9,5.9,156,E
+00009b60: 2c35 2e36 2c32 3332 2c36 2e35 2c32 2e38  ,5.6,232,6.5,2.8
+00009b70: 312c 3137 3030 2c31 3739 352c 3234 3130  1,1700,1795,2410
+00009b80: 2c31 3030 2c39 302c 3332 312e 322c 3334  ,100,90,321.2,34
+00009b90: 302e 3637 3936 3131 372c 5b34 2e37 312d  0.6796117,[4.71-
+00009ba0: 2033 2e31 342d 2032 2e31 312d 2031 2e36   3.14- 2.11- 1.6
+00009bb0: 372d 2031 2e32 392d 2031 2e30 2d20 302e  7- 1.29- 1.0- 0.
+00009bc0: 3834 2d20 302e 3637 5d2c 3137 3439 2e37  84- 0.67],1749.7
+00009bd0: 3735 2c31 3832 342e 3737 352c 3138 3439  75,1824.775,1849
+00009be0: 2e37 3735 2c31 3831 302c 332e 3132 3433  .775,1810,3.1243
+00009bf0: 3431 2c4a 0d0a 3236 3731 322c 4a2c 2c79  41,J..26712,J,,y
+00009c00: 6573 2c79 6573 2c79 6573 2c79 6573 2c79  es,yes,yes,yes,y
+00009c10: 6573 2c79 6573 2c6e 6f2c 7965 732c 7965  es,yes,no,yes,ye
+00009c20: 732c 7965 732c 6879 6272 6964 2c70 6574  s,yes,hybrid,pet
+00009c30: 726f 6c2c 3130 342c 3236 352c 6672 6f6e  rol,104,265,fron
+00009c40: 742c 312e 3536 2c6c 6974 6869 756d 2d69  t,1.56,lithium-i
+00009c50: 6f6e 2c32 3430 2c2c 7379 6e63 6872 6f6e  on,240,,synchron
+00009c60: 6f75 7320 6d6f 746f 7220 2c31 3730 2c31  ous motor ,170,1
+00009c70: 2c33 322c 2c2c 312e 3534 352c 342e 3335  ,32,,,1.545,4.35
+00009c80: 352c 322e 372c 312e 3830 352c 302e 3136  5,2.7,1.805,0.16
+00009c90: 2c31 3538 302c 7265 6775 6c61 722c 342c  ,1580,regular,4,
+00009ca0: 2c69 6e6a 6563 7469 6f6e 2c34 352c 3537  ,injection,45,57
+00009cb0: 3030 2c37 372c 3430 3030 2c31 3437 2c6e  00,77,4000,147,n
+00009cc0: 6f2c 342c 7375 762f 6372 6f73 736f 7665  o,4,suv/crossove
+00009cd0: 722c 352c 6176 6169 6c61 626c 652c 3333  r,5,available,33
+00009ce0: 3039 352c 352c 3230 3136 2c61 7574 6f6d  095,5,2016,autom
+00009cf0: 6174 6963 2c31 312e 352c 342e 342c 3130  atic,11.5,4.4,10
+00009d00: 312c 412c 342e 352c 3136 322c 342e 342c  1,A,4.5,162,4.4,
+00009d10: 332e 3233 2c32 3430 302c 3134 3231 2c31  3.23,2400,1421,1
+00009d20: 3933 302c 2c39 372c 3332 392e 3835 2c33  930,,97,329.85,3
+00009d30: 3230 2e32 3432 3731 3834 2c5b 332e 3837  20.2427184,[3.87
+00009d40: 2d20 322e 3232 2d20 312e 3337 2d20 302e  - 2.22- 1.37- 0.
+00009d50: 3936 2d20 302e 3933 2d20 302e 3737 5d2c  96- 0.93- 0.77],
+00009d60: 3134 3231 2c31 3439 362c 3135 3231 2c31  1421,1496,1521,1
+00009d70: 3437 302c 322e 3738 3837 3235 2c0d 0a32  470,2.788725,..2
+00009d80: 3637 3133 2c4a 2c2c 7965 732c 7965 732c  6713,J,,yes,yes,
+00009d90: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+00009da0: 6e6f 2c79 6573 2c79 6573 2c79 6573 2c66  no,yes,yes,yes,f
+00009db0: 7565 6c20 656e 6769 6e65 2c70 6574 726f  uel engine,petro
+00009dc0: 6c2c 3737 2c32 3635 2c66 726f 6e74 2c31  l,77,265,front,1
+00009dd0: 2e35 362c 6c69 7468 6975 6d2d 696f 6e2c  .56,lithium-ion,
+00009de0: 3234 302c 2c73 796e 6368 726f 6e6f 7573  240,,synchronous
+00009df0: 206d 6f74 6f72 202c 3137 302c 312c 3332   motor ,170,1,32
+00009e00: 2c2c 2c31 2e35 3435 2c34 2e33 3535 2c32  ,,,1.545,4.355,2
+00009e10: 2e37 2c31 2e38 3035 2c30 2e31 362c 3135  .7,1.805,0.16,15
+00009e20: 3830 2c72 6567 756c 6172 2c34 2c2c 696e  80,regular,4,,in
+00009e30: 6a65 6374 696f 6e2c 3435 2c35 3730 302c  jection,45,5700,
+00009e40: 3737 2c34 3030 302c 3134 372c 6e6f 2c34  77,4000,147,no,4
+00009e50: 2c73 7576 2f63 726f 7373 6f76 6572 2c35  ,suv/crossover,5
+00009e60: 2c61 7661 696c 6162 6c65 2c33 3330 3935  ,available,33095
+00009e70: 2c35 2c32 3031 362c 6175 746f 6d61 7469  ,5,2016,automati
+00009e80: 632c 3131 2e35 2c34 2e34 2c31 3031 2c41  c,11.5,4.4,101,A
+00009e90: 2c34 2e35 2c31 3632 2c34 2e34 2c34 2e34  ,4.5,162,4.4,4.4
+00009ea0: 3338 2c32 3430 302c 3134 3231 2c31 3933  38,2400,1421,193
+00009eb0: 302c 2c39 372c 3332 392e 3835 2c33 3230  0,,97,329.85,320
+00009ec0: 2e32 3432 3731 3834 2c5b 332e 3837 2d20  .2427184,[3.87- 
+00009ed0: 322e 3232 2d20 312e 3337 2d20 302e 3936  2.22- 1.37- 0.96
+00009ee0: 2d20 302e 3933 2d20 302e 3737 5d2c 3134  - 0.93- 0.77],14
+00009ef0: 3231 2c31 3439 362c 3135 3231 2c31 3437  21,1496,1521,147
+00009f00: 302c 322e 3738 3837 3235 2c0d 0a32 3637  0,2.788725,..267
+00009f10: 3134 2c4a 2c2c 7965 732c 7965 732c 7965  14,J,,yes,yes,ye
+00009f20: 732c 7965 732c 7965 732c 7965 732c 6e6f  s,yes,yes,yes,no
+00009f30: 2c79 6573 2c79 6573 2c79 6573 2c65 6c65  ,yes,yes,yes,ele
+00009f40: 6374 7269 6320 656e 6769 6e65 2c65 6c65  ctric engine,ele
+00009f50: 6374 7269 6369 7479 2c31 3034 2c32 3635  ctricity,104,265
+00009f60: 2c66 726f 6e74 2c31 2e35 362c 6c69 7468  ,front,1.56,lith
+00009f70: 6975 6d2d 696f 6e2c 3234 302c 2c73 796e  ium-ion,240,,syn
+00009f80: 6368 726f 6e6f 7573 206d 6f74 6f72 202c  chronous motor ,
+00009f90: 3137 302c 312c 3332 2c2c 2c31 2e35 3435  170,1,32,,,1.545
+00009fa0: 2c34 2e33 3535 2c32 2e37 2c31 2e38 3035  ,4.355,2.7,1.805
+00009fb0: 2c30 2e31 362c 3135 3830 2c72 6567 756c  ,0.16,1580,regul
+00009fc0: 6172 2c34 2c2c 696e 6a65 6374 696f 6e2c  ar,4,,injection,
+00009fd0: 3435 2c35 3730 302c 3737 2c34 3030 302c  45,5700,77,4000,
+00009fe0: 3134 372c 6e6f 2c34 2c73 7576 2f63 726f  147,no,4,suv/cro
+00009ff0: 7373 6f76 6572 2c35 2c61 7661 696c 6162  ssover,5,availab
+0000a000: 6c65 2c33 3330 3935 2c35 2c32 3031 362c  le,33095,5,2016,
+0000a010: 6175 746f 6d61 7469 632c 3131 2e35 2c34  automatic,11.5,4
+0000a020: 2e34 2c31 3031 2c41 2c34 2e35 2c31 3632  .4,101,A,4.5,162
+0000a030: 2c34 2e34 2c33 2e32 332c 3234 3030 2c31  ,4.4,3.23,2400,1
+0000a040: 3432 312c 3139 3330 2c2c 3937 2c33 3239  421,1930,,97,329
+0000a050: 2e38 352c 3332 302e 3234 3237 3138 342c  .85,320.2427184,
+0000a060: 5b33 2e38 372d 2032 2e32 322d 2031 2e33  [3.87- 2.22- 1.3
+0000a070: 372d 2030 2e39 362d 2030 2e39 332d 2030  7- 0.96- 0.93- 0
+0000a080: 2e37 375d 2c31 3432 312c 3134 3936 2c31  .77],1421,1496,1
+0000a090: 3532 312c 3134 3730 2c32 2e37 3838 3732  521,1470,2.78872
+0000a0a0: 352c 0d0a 3236 3731 352c 4a2c 2c79 6573  5,..26715,J,,yes
+0000a0b0: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
+0000a0c0: 2c79 6573 2c6e 6f2c 7965 732c 7965 732c  ,yes,no,yes,yes,
+0000a0d0: 7965 732c 6879 6272 6964 2c70 6574 726f  yes,hybrid,petro
+0000a0e0: 6c2c 3130 342c 3236 352c 6672 6f6e 742c  l,104,265,front,
+0000a0f0: 312e 3536 2c6c 6974 6869 756d 2d69 6f6e  1.56,lithium-ion
+0000a100: 2c32 3430 2c2c 7379 6e63 6872 6f6e 6f75  ,240,,synchronou
+0000a110: 7320 6d6f 746f 7220 2c31 3730 2c31 2c33  s motor ,170,1,3
+0000a120: 322c 2c2c 312e 3534 352c 342e 3335 352c  2,,,1.545,4.355,
+0000a130: 322e 372c 312e 3830 352c 302e 3136 2c31  2.7,1.805,0.16,1
+0000a140: 3538 302c 7265 6775 6c61 722c 342c 2c69  580,regular,4,,i
+0000a150: 6e6a 6563 7469 6f6e 2c34 352c 3537 3030  njection,45,5700
+0000a160: 2c37 372c 3430 3030 2c31 3437 2c6e 6f2c  ,77,4000,147,no,
+0000a170: 342c 7375 762f 6372 6f73 736f 7665 722c  4,suv/crossover,
+0000a180: 352c 6176 6169 6c61 626c 652c 3333 3039  5,available,3309
+0000a190: 352c 352c 3230 3136 2c6d 616e 7561 6c2c  5,5,2016,manual,
+0000a1a0: 3131 2e35 2c34 2e34 2c31 3031 2c41 2c34  11.5,4.4,101,A,4
+0000a1b0: 2e35 2c31 3632 2c34 2e34 2c33 2e32 332c  .5,162,4.4,3.23,
+0000a1c0: 3234 3030 2c31 3432 312c 3139 3330 2c2c  2400,1421,1930,,
+0000a1d0: 3937 2c33 3239 2e38 352c 3332 302e 3234  97,329.85,320.24
+0000a1e0: 3237 3138 342c 5b33 2e38 372d 2032 2e32  27184,[3.87- 2.2
+0000a1f0: 322d 2031 2e33 372d 2030 2e39 362d 2030  2- 1.37- 0.96- 0
+0000a200: 2e39 332d 2030 2e37 375d 2c31 3432 312c  .93- 0.77],1421,
+0000a210: 3134 3936 2c31 3532 312c 3134 3730 2c32  1496,1521,1470,2
+0000a220: 2e37 3838 3732 352c 0d0a 3236 3731 362c  .788725,..26716,
+0000a230: 4a2c 2c79 6573 2c79 6573 2c79 6573 2c79  J,,yes,yes,yes,y
+0000a240: 6573 2c79 6573 2c79 6573 2c6e 6f2c 7965  es,yes,yes,no,ye
+0000a250: 732c 7965 732c 7965 732c 6879 6272 6964  s,yes,yes,hybrid
+0000a260: 2c70 6574 726f 6c2c 3132 312e 352c 3236  ,petrol,121.5,26
+0000a270: 352c 6672 6f6e 742c 312e 3536 2c6c 6974  5,front,1.56,lit
+0000a280: 6869 756d 2d69 6f6e 2c32 3430 2c2c 7379  hium-ion,240,,sy
+0000a290: 6e63 6872 6f6e 6f75 7320 6d6f 746f 7220  nchronous motor 
+0000a2a0: 2c31 3730 2c31 2c34 342e 352c 2c2c 312e  ,170,1,44.5,,,1.
+0000a2b0: 3534 352c 342e 3335 352c 322e 372c 312e  545,4.355,2.7,1.
+0000a2c0: 3830 352c 302e 3136 2c31 3538 302c 7265  805,0.16,1580,re
+0000a2d0: 6775 6c61 722c 342c 2c69 6e6a 6563 7469  gular,4,,injecti
+0000a2e0: 6f6e 2c34 352c 3537 3030 2c37 372c 3430  on,45,5700,77,40
+0000a2f0: 3030 2c31 3437 2c6e 6f2c 342c 7375 762f  00,147,no,4,suv/
+0000a300: 6372 6f73 736f 7665 722c 352c 6176 6169  crossover,5,avai
+0000a310: 6c61 626c 652c 3333 3039 352c 352c 3230  lable,33095,5,20
+0000a320: 3136 2c61 7574 6f6d 6174 6963 2c31 312e  16,automatic,11.
+0000a330: 352c 342e 342c 3130 312c 412c 342e 352c  5,4.4,101,A,4.5,
+0000a340: 3136 322c 342e 342c 342e 3433 382c 3234  162,4.4,4.438,24
+0000a350: 3030 2c31 3432 312c 3139 3330 2c2c 3937  00,1421,1930,,97
+0000a360: 2c33 3239 2e38 352c 3332 302e 3234 3237  ,329.85,320.2427
+0000a370: 3138 342c 5b33 2e38 372d 2032 2e32 322d  184,[3.87- 2.22-
+0000a380: 2031 2e33 372d 2030 2e39 362d 2030 2e39   1.37- 0.96- 0.9
+0000a390: 332d 2030 2e37 375d 2c31 3432 312c 3134  3- 0.77],1421,14
+0000a3a0: 3936 2c31 3532 312c 3134 3730 2c32 2e37  96,1521,1470,2.7
+0000a3b0: 3838 3732 352c 0d0a 3236 3731 372c 4a2c  88725,..26717,J,
+0000a3c0: 2c79 6573 2c79 6573 2c79 6573 2c79 6573  ,yes,yes,yes,yes
+0000a3d0: 2c79 6573 2c79 6573 2c6e 6f2c 7965 732c  ,yes,yes,no,yes,
+0000a3e0: 7965 732c 7965 732c 656c 6563 7472 6963  yes,yes,electric
+0000a3f0: 2065 6e67 696e 652c 656c 6563 7472 6963   engine,electric
+0000a400: 6974 792c 3434 2e35 2c32 3635 2c66 726f  ity,44.5,265,fro
+0000a410: 6e74 2c31 2e35 362c 6c69 7468 6975 6d2d  nt,1.56,lithium-
+0000a420: 696f 6e2c 3234 302c 2c73 796e 6368 726f  ion,240,,synchro
+0000a430: 6e6f 7573 206d 6f74 6f72 202c 3137 302c  nous motor ,170,
+0000a440: 312c 3434 2e35 2c2c 2c31 2e35 3435 2c34  1,44.5,,,1.545,4
+0000a450: 2e33 3535 2c32 2e37 2c31 2e38 3035 2c30  .355,2.7,1.805,0
+0000a460: 2e31 362c 3135 3830 2c72 6567 756c 6172  .16,1580,regular
+0000a470: 2c34 2c2c 696e 6a65 6374 696f 6e2c 3435  ,4,,injection,45
+0000a480: 2c35 3730 302c 3737 2c34 3030 302c 3134  ,5700,77,4000,14
+0000a490: 372c 6e6f 2c34 2c73 7576 2f63 726f 7373  7,no,4,suv/cross
+0000a4a0: 6f76 6572 2c35 2c61 7661 696c 6162 6c65  over,5,available
+0000a4b0: 2c33 3330 3935 2c35 2c32 3031 362c 6175  ,33095,5,2016,au
+0000a4c0: 746f 6d61 7469 632c 3131 2e35 2c34 2e34  tomatic,11.5,4.4
+0000a4d0: 2c31 3031 2c41 2c34 2e35 2c31 3632 2c34  ,101,A,4.5,162,4
+0000a4e0: 2e34 2c34 2e34 3338 2c32 3430 302c 3134  .4,4.438,2400,14
+0000a4f0: 3231 2c31 3933 302c 2c39 372c 3332 392e  21,1930,,97,329.
+0000a500: 3835 2c33 3230 2e32 3432 3731 3834 2c5b  85,320.2427184,[
+0000a510: 332e 3837 2d20 322e 3232 2d20 312e 3337  3.87- 2.22- 1.37
+0000a520: 2d20 302e 3936 2d20 302e 3933 2d20 302e  - 0.96- 0.93- 0.
+0000a530: 3737 5d2c 3134 3231 2c31 3439 362c 3135  77],1421,1496,15
+0000a540: 3231 2c31 3437 302c 322e 3738 3837 3235  21,1470,2.788725
+0000a550: 2c0d 0a32 3637 3138 2c4a 2c2c 7965 732c  ,..26718,J,,yes,
+0000a560: 7965 732c 7965 732c 7965 732c 7965 732c  yes,yes,yes,yes,
+0000a570: 7965 732c 6e6f 2c79 6573 2c79 6573 2c79  yes,no,yes,yes,y
+0000a580: 6573 2c66 7565 6c20 656e 6769 6e65 2c70  es,fuel engine,p
+0000a590: 6574 726f 6c2c 3132 312e 352c 3236 352c  etrol,121.5,265,
+0000a5a0: 6672 6f6e 742c 312e 3536 2c6c 6974 6869  front,1.56,lithi
+0000a5b0: 756d 2d69 6f6e 2c32 3430 2c2c 7379 6e63  um-ion,240,,sync
+0000a5c0: 6872 6f6e 6f75 7320 6d6f 746f 7220 2c31  hronous motor ,1
+0000a5d0: 3730 2c31 2c33 322c 2c2c 312e 3534 352c  70,1,32,,,1.545,
+0000a5e0: 342e 3335 352c 322e 372c 312e 3830 352c  4.355,2.7,1.805,
+0000a5f0: 302e 3136 2c31 3538 302c 7265 6775 6c61  0.16,1580,regula
+0000a600: 722c 342c 2c69 6e6a 6563 7469 6f6e 2c34  r,4,,injection,4
+0000a610: 352c 3537 3030 2c37 372c 3430 3030 2c31  5,5700,77,4000,1
+0000a620: 3437 2c6e 6f2c 342c 7375 762f 6372 6f73  47,no,4,suv/cros
+0000a630: 736f 7665 722c 352c 6176 6169 6c61 626c  sover,5,availabl
+0000a640: 652c 3333 3039 352c 352c 3230 3136 2c61  e,33095,5,2016,a
+0000a650: 7574 6f6d 6174 6963 2c31 312e 352c 342e  utomatic,11.5,4.
+0000a660: 342c 3130 312c 412c 342e 352c 3136 322c  4,101,A,4.5,162,
+0000a670: 342e 342c 332e 3233 2c32 3430 302c 3134  4.4,3.23,2400,14
+0000a680: 3231 2c31 3933 302c 2c39 372c 3332 392e  21,1930,,97,329.
+0000a690: 3835 2c33 3230 2e32 3432 3731 3834 2c5b  85,320.2427184,[
+0000a6a0: 332e 3837 2d20 322e 3232 2d20 312e 3337  3.87- 2.22- 1.37
+0000a6b0: 2d20 302e 3936 2d20 302e 3933 2d20 302e  - 0.96- 0.93- 0.
+0000a6c0: 3737 5d2c 3134 3231 2c31 3439 362c 3135  77],1421,1496,15
+0000a6d0: 3231 2c31 3437 302c 322e 3738 3837 3235  21,1470,2.788725
+0000a6e0: 2c0d 0a                                  ,..
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/euro_segment.py` & `co2mpas_driver-1.3.3/co2mpas_driver/euro_segment.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_gear_shifting.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_gear_shifting.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_light_co2mpas.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_light_co2mpas.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_simulation.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_simulation.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_varying_des_speed.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/sample_veh_specs_collection.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_veh_specs_collection.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/examples/test.py` & `co2mpas_driver-1.3.3/co2mpas_driver/examples/test.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/load.py` & `co2mpas_driver-1.3.3/co2mpas_driver/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import logging
 import numpy as np
 import os.path as osp
+from pathlib import Path
 import schedula as sh
 
 log = logging.getLogger(__name__)
 dsp = sh.BlueDispatcher(name="load", description="Read/merge/parse input data.")
 
 
 def check_ext(fpath, *args, ext=("xls", "xlsx")):
@@ -62,15 +63,15 @@
     :rtype: int
     """
     return raw_data["config"]["vehicle_id"]
 
 
 dsp.add_data(
     "db_path",
-    osp.join(osp.dirname(__file__), "db", "EuroSegmentCar_cleaned.csv"),
+    Path(osp.dirname(__file__)).joinpath("db").joinpath("EuroSegmentCar_cleaned.csv"),
     sh.inf(1, 0),
 )
 
 
 @sh.add_function(dsp, outputs=["db_path"])
 def get_db_path(raw_data):
     """
@@ -80,15 +81,22 @@
         Raw data of input file.
     :type raw_data: dict
 
     :return:
         Data base file path.
     :rtype: str
     """
-    return raw_data.get("config", {}).get("db_path", sh.NONE)
+    if raw_data.get("config", {}).get("db_path", sh.NONE) == sh.NONE:
+        return (
+            Path(osp.dirname(__file__))
+            .joinpath("db")
+            .joinpath("EuroSegmentCar_cleaned.csv")
+        )
+    else:
+        return raw_data.get("config", {}).get("db_path", sh.NONE)
 
 
 _db_map = {
     "Transmission  / Gear ratio-Final drive": "final_drive_ratio",
     "Transmission  / Gear ratio-Gear Box Ratios": "gear_box_ratios",
     "Weights-Empty mass": "vehicle_mass",
     "Performance-Top speed": "vehicle_max_speed",
@@ -97,24 +105,27 @@
     "Exterior sizes-Height": "car_height",
     "Weights-Unladen mass": "kerb_weight",
     "Exterior sizes-Wheelbase": "wheelbase",
     "Drive-Wheel drive": "car_type",
     "Drive-Fuel": "fuel_type",
     "Chassis-Rolling Radius Dynamic": "r_dynamic",
     "Fuel Engine-Max torque": "engine_max_torque",
+    "Electric Engine-Max torque": "motor_max_torque",
     "Fuel Engine-Stroke": "fuel_engine_stroke",
-    "Drive-Total max power": "max_power",
+    "Fuel Engine-Max power": "engine_max_power",
+    "Electric Engine-Total max power": "motor_max_power",
     "Fuel Engine-Turbo": "fuel_turbo",
     "Fuel Engine-Capacity": "fuel_eng_capacity",
     "General Specifications-Transmission": "gearbox_type",
-    "Fuel Engine-Max power": "engine_max_power",
-    "Electric Engine-Total max power": "motor_max_power",
-    "Electric Engine-Max torque": "motor_max_torque",
+    "Drive-Total max power": "max_power",
     "Chassis-Rolling Radius Static": "tyre_radius",
     "Fuel Engine-Max power RPM": "engine_max_speed_at_max_power",
+    "Electric Engine-Battery capacity": "drive_battery_capacity",  # kwh
+    "Electric Engine-Battery voltage": "drive_battery_voltage",
+    "Drive-Drive system": "fuel_mode",
 }
 
 
 @sh.add_function(dsp, outputs=["vehicle_db"])
 def load_vehicle_db(db_path):
     """
     Load vehicle data base.
@@ -125,27 +136,29 @@
 
     :return:
         Vehicle database.
     :rtype: dict
     """
     import pandas as pd
 
-    df = pd.read_csv(db_path, encoding="ISO-8859-1", index_col=0)
+    df = pd.read_csv(
+        db_path,
+        index_col=0,
+        encoding="utf-8-sig",
+    )
     df = df[list(_db_map)].rename(columns=_db_map)
 
     df["gear_box_ratios"] = (
-        df["gear_box_ratios"]
-        .fillna("[]")
-        .apply(lambda x: [float(v) for v in x[1:-1].split("-") if v != ""])
+        df["gear_box_ratios"].fillna("[1, ]").apply(lambda x: eval(x.replace("-", ",")))
     )
+
     df.loc[df["fuel_type"] == "petrol", "ignition_type"] = "positive"
     df.loc[df["fuel_type"] == "diesel", "ignition_type"] = "compression"
     b = df["fuel_type"] == "electricity"
     df.loc[b, ["ignition_type"]] = "electricity"
-    df.loc[b, ["gear_box_ratios"]] = 1
     df["tyre_radius"] /= 1000  # meters.
     df["driveline_slippage"] = 0
 
     b = df["gearbox_type"] == "automatic"
     # b |= df['gearbox_type'] == 'single-speed fixed gear'
     df["transmission"] = np.where(b, "automatic", "manual")
     df["driveline_efficiency"] = np.where(b, 0.9, 0.93)
@@ -168,14 +181,18 @@
     r[df["car_type"] == "rear"] = 4
     df["car_type"] = r
 
     b = df["ignition_type"] == "positive"
     df["idle_engine_speed_median"] = np.where(b, 750, 850)
     df["idle_engine_speed_std"] = 50
     df["r_dynamic"] /= 1000
+    df["drive_battery_capacity"] *= 1000 / df["drive_battery_voltage"]
+
+    df.loc[df["fuel_mode"] == "fuel engine", "motor_max_power"] = 0
+    df.loc[df["fuel_mode"] == "fuel engine", "motor_max_torque"] = 0
 
     return df.to_dict("index")
 
 
 @sh.add_function(dsp, outputs=["vehicle_inputs"])
 def get_vehicle_inputs(vehicle_id, vehicle_db):
     """
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/model/__init__.py` & `co2mpas_driver-1.3.3/co2mpas_driver/model/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright 2019 European Commission (JRC);
 # Licensed under the EUPL (the 'Licence');
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 """
 Functions and a model `dsp` to process a CO2MPAS input file.
+
+Sub-Modules:
+.. currentmodule:: co2mpas_driver.model
+.. autosummary::
+    :nosignatures:
+    :toctree: model/
+    co2mpas
+    simulation
 """
 import numpy as np
+import functools
 import schedula as sh
 from .driver import Driver as dr
 from co2mpas_driver.model.co2mpas import (
     get_full_load,
     calculate_full_load_speeds_and_powers,
     calculate_full_load_torques,
 )
@@ -109,16 +118,168 @@
 
     return speed_per_gear, acc_per_gear
 
 
 dsp.add_data("degree", 2)
 
 
+@sh.add_function(dsp, outputs=["motor_full_load_speeds", "motor_full_load_torques"])
+def calculate_motor_full_load_speeds_and_torques(
+    motor_max_power,
+    motor_max_torque,
+    vehicle_max_speed,
+    fuel_mode,
+    final_drive_ratio,
+    gear_box_ratios,
+    tyre_radius,
+    driveline_slippage,
+):
+    if fuel_mode == "fuel engine":
+        return [0] * 2
+
+    motor_base_speed = (
+        motor_max_power * 1000 * (motor_max_torque / 60 * 2 * np.pi) ** -1
+    )  # rpm
+    motor_max_speed = (
+        vehicle_max_speed
+        * (60 * final_drive_ratio * gear_box_ratios[0])
+        / (1 - driveline_slippage)
+        / (2 * np.pi * tyre_radius)
+    )  # rpm
+    if motor_max_speed > 9000:
+        motor_max_speed = 9000
+    motor_full_load_speeds = list(np.arange(0, motor_max_speed, 50)) + [motor_max_speed]
+    motor_full_load_torque = []
+    for k in range(len(motor_full_load_speeds)):
+        if 0 <= motor_full_load_speeds[k] <= motor_base_speed:
+            motor_full_load_torque.append(motor_max_torque)
+        elif motor_full_load_speeds[k] > motor_base_speed:
+            motor_full_load_torque.append(
+                (6e4 * motor_max_power) / (2 * np.pi * motor_full_load_speeds[k])
+            )
+
+    return motor_full_load_speeds, motor_full_load_torque
+
+
+@sh.add_function(dsp, outputs=["motor_full_load_powers"])
+def calculate_motor_full_load_powers(motor_full_load_speeds, motor_full_load_torques):
+    return (
+        np.array(motor_full_load_torques)
+        * np.array(motor_full_load_speeds)
+        * 2
+        * np.pi
+        / 60
+        / 1000
+    )
+
+
+def calculate_full_load_curve(xp, fp, fuel_mode):
+    _xp = xp
+    _fp = fp
+    if fuel_mode == "fuel engine":
+        _xp = [xp]
+        _fp = [fp]
+    func = functools.partial(np.interp, xp=_xp, fp=_fp, left=_fp[0], right=_fp[-1])
+    return func
+
+
+dsp.add_func(
+    calculate_full_load_curve,
+    inputs=["motor_full_load_speeds", "motor_full_load_powers", "fuel_mode"],
+    outputs=["motor_full_load_curve"],
+)
+
+
+# Speed and acceleration ranges and points for each gear
+@sh.add_function(dsp, outputs=["motor_speed_per_gear", "motor_acc_per_gear"])
+def get_speeds_n_accelerations_per_gear_electric(
+    gear_box_ratios,
+    tyre_radius,
+    driveline_slippage,
+    final_drive_ratio,
+    driveline_efficiency,
+    vehicle_mass,
+    motor_full_load_speeds,
+    motor_full_load_torques,
+    fuel_mode,
+):
+    """
+    Speed and acceleration points per gear are calculated based on
+    full load curve, new version works with array and
+    forbid acceleration over the maximum vehicle speed.
+
+    :param gear_box_ratios:
+        Gear box ratio.
+    :type gear_box_ratios: list
+
+    :param idle_engine_speed:
+        Idle engine speed.
+    :type idle_engine_speed: tuple
+
+    :param tyre_radius:
+        Tyre radius.
+    :type tyre_radius: float
+
+    :param driveline_slippage:
+        Drive line slippage.
+    :type driveline_slippage: int
+
+    :param final_drive_ratio:
+        Final drive.
+    :type final_drive_ratio: float
+
+    :param driveline_efficiency:
+        Driveline efficiency.
+    :type driveline_efficiency: float
+
+    :param vehicle_mass:
+        Vehicle mass.
+    :type vehicle_mass: float
+
+    :param full_load_speeds:
+        Full load speeds.
+    :type motor_full_load_speeds: numpy.array
+
+    :param full_load_torques:
+    :type motor_full_load_torques: numpy.array
+
+    :return: speed_per_gear, acc_per_gear
+    """
+
+    if fuel_mode == "fuel engine":
+        return [0] * 2
+
+    motor_full_load_speeds = np.array(motor_full_load_speeds)
+    motor_full_load_torque = np.array(motor_full_load_torques)
+
+    motor_speed_per_gear, motor_acc_per_gear = [], []
+    for j in range(len(gear_box_ratios)):
+        motor_speed_per_gear.append([])
+        motor_acc_per_gear.append([])
+        for i in range(len(motor_full_load_speeds)):
+            motor_speed_per_gear[j].append(
+                2
+                * np.pi
+                * tyre_radius
+                * motor_full_load_speeds[i]
+                * (1 - driveline_slippage)
+                / (60 * final_drive_ratio * gear_box_ratios[j])
+            )
+            motor_acc_per_gear[j].append(
+                motor_full_load_torque[i]
+                * (final_drive_ratio * gear_box_ratios[j])
+                * driveline_efficiency
+                / (tyre_radius * vehicle_mass)
+            )
+
+    return motor_speed_per_gear, motor_acc_per_gear
+
+
 @sh.add_function(dsp, outputs=["coefs_per_gear"])
-def get_tan_coefs(speed_per_gear, acc_per_gear, degree):
+def get_tan_coefs(speed_per_gear, acc_per_gear, degree, fuel_mode):
     """
     Calculate the coefficients of the polynomial for each gear
     Full load curve is fitted to a polynomial of degree.
 
     :param speed_per_gear:
         Speed per gear.
     :type speed_per_gear: list[tuple[float]]
@@ -131,36 +292,24 @@
         Degree.
     :type degree: int
 
     :return: coefs_per_gear:
         The coefficients of the polynomial for each gear.
     :rtype: list[tuple[float]]]
     """
+    if fuel_mode == "electric engine":
+        return [sh.NONE]
     it = zip(speed_per_gear, acc_per_gear)
     return [np.polyfit(s, a, degree) for s, a in it]
 
 
-dsp.add_function(
-    function=sh.bypass, inputs=["motor_max_power"], outputs=["engine_max_power"]
-)
-
-
-@sh.add_function(dsp, outputs=["poly_spline", "start", "stop"])
-def ev_curve(
-    fuel_type,
-    engine_max_power,
-    tyre_radius,
-    motor_max_torque,
-    final_drive_ratio,
-    driveline_efficiency,
-    vehicle_mass,
-    vehicle_max_speed,
-):
+@sh.add_function(dsp, outputs=["poly_spline_electric"])
+def ev_curve(fuel_mode, gear_box_ratios, motor_speed_per_gear, motor_acc_per_gear):
     """
-    Full load curve of EVs (based on Yinglong).
+    electric poly_spline (based on Yinglong).
 
     :param fuel_type:
         Fuel type.
     :type fuel_type: str
 
     :param engine_max_power:
         Engine maximum power.
@@ -190,43 +339,41 @@
         Vehicle maximum speed. [m/s]
     :type vehicle_max_speed: int
 
     :return:
         Acceleration potential curves of Electric Vehicle
     :rtype: list[tuple[float]]]
     """
-    if fuel_type != "electricity":
-        return [sh.NONE] * 3
+    if fuel_mode == "fuel engine":
+        return 0
     from scipy.interpolate import CubicSpline
 
-    eff, fdr = driveline_efficiency, final_drive_ratio
+    cs_motor_acc_per_gear = []
+    for j in range(len(gear_box_ratios)):
+        a = np.round((motor_speed_per_gear[j][0]), 2) - 0.01
+        b = np.round((motor_speed_per_gear[j][-1]), 2) + 0.01
+        prefix_list = [a - k * 0.1 for k in range(10, -1, -1)]
+        suffix_list = [b + k * 0.1 for k in range(0, 11, 1)]
+        cs_motor_acc_per_gear.append(
+            CubicSpline(
+                prefix_list + motor_speed_per_gear[j] + suffix_list,
+                [motor_acc_per_gear[j][0]] * len(prefix_list)
+                + motor_acc_per_gear[j]
+                + [motor_acc_per_gear[j][-1]] * len(suffix_list),
+            )
+        )
 
-    max_a = motor_max_torque * fdr * eff / (tyre_radius * vehicle_mass)  # m/s2
-    s = np.arange(0, vehicle_max_speed + 0.1, 0.1)  # m/s
-    a = np.round((s[0]), 2) - 0.01
-    b = np.round((s[-1]), 2) + 0.01
-    prefix = np.asarray([a - k * 0.1 for k in range(10, -1, -1)])
-    suffix = np.asarray([b + k * 0.1 for k in range(0, 11, 1)])
+    return cs_motor_acc_per_gear
 
-    with np.errstate(divide="ignore"):
-        a = (engine_max_power * 1e3 * eff / (s * vehicle_mass)).clip(0, max_a)
 
-    return (
-        [
-            CubicSpline(
-                np.append(np.append(prefix, s), suffix),
-                np.append(
-                    np.append(np.repeat(a[0], len(prefix)), a),
-                    np.repeat(a[-1], len(suffix)),
-                ),
-            )
-        ],
-        [s[0]],
-        [s[-1]],
-    )
+@sh.add_function(dsp, outputs=["poly_spline"])
+def electric_poly_spline(poly_spline_electric, fuel_mode):
+    if fuel_mode != "electric engine":
+        return sh.NONE
+    return poly_spline_electric
 
 
 @sh.add_function(dsp, inputs_kwargs=True, outputs=["poly_spline"])
 def get_cubic_splines_of_speed_acceleration_relationship(
     speed_per_gear, acc_per_gear, use_cubic=True
 ):
     """
@@ -326,20 +473,46 @@
     :type sp_bins: numpy.array
 
     :rtype: list[tuple[float]]]
     """
     return [acc(sp_bins) for acc in poly_spline]
 
 
+# Start/stop speed for each gear for the electric
+@sh.add_function(dsp, outputs=["start_electric", "stop_electric"])
+def get_start_stop_electric(motor_speed_per_gear, fuel_mode):
+    if fuel_mode == "fuel engine":
+        return [0] * 2
+
+    _start = [i[0] for i in motor_speed_per_gear]
+    _stop = [i[-1] for i in motor_speed_per_gear]
+    return _start, _stop
+
+
+@sh.add_function(
+    dsp,
+    outputs=["start", "stop"],
+)
+def electric_start_stop(start_electric, stop_electric, fuel_mode):
+    if fuel_mode != "electric engine":
+        return [sh.NONE] * 2
+    return start_electric, stop_electric
+
+
 # Start/stop speed for each gear
 @sh.add_function(
     dsp, outputs=["start", "stop", "speed_per_gear_updated", "acc_per_gear_updated"]
 )
 def get_start_stop(
-    gear_box_ratios, acc_per_gear, vehicle_max_speed, speed_per_gear, poly_spline
+    gear_box_ratios,
+    acc_per_gear,
+    vehicle_max_speed,
+    speed_per_gear,
+    poly_spline,
+    fuel_mode,
 ):
     """
     Calculate Speed boundaries for each gear.
 
     :param gear_box_ratios:
         Gear box ratios.
     :type gear_box_ratios: list
@@ -360,14 +533,18 @@
         Poly spline.
     :type poly_spline: list
 
     :return:
         Start and Stop for each gear.
     :rtype: numpy.array, numpy.array
     """
+
+    if fuel_mode == "electric engine":
+        return [sh.NONE] * 4
+
     # To ensure that a higher gear starts from higher speed
     for j in range(len(gear_box_ratios) - 1, 0, -1):
         for k in range(len(speed_per_gear[j])):
             if speed_per_gear[j - 1][0] < speed_per_gear[j][0]:
                 break
             else:
                 # If the gear ratios are not declining,
@@ -510,15 +687,15 @@
     from .co2mpas import veh_resistances
 
     return veh_resistances(f0, f1, f2, sp_bins, vehicle_mass, angle_slopes, g)
 
 
 # The maximum force that the vehicle can have on the road
 @sh.add_function(dsp, outputs=["Alimit"])
-def Armax(car_type, vehicle_mass, engine_max_power, road_type=1):
+def Armax(car_type, vehicle_mass, max_power, road_type=1):
     """
     Calculate the maximum acceleration possible for the vehicle object my_car,
     under road_type conditions.
 
     :param car_type:
         Car type.
     :type car_type: int
@@ -540,22 +717,33 @@
     :rtype: float
     """
 
     mass = {2: 0.6, 4: 0.45}.get(car_type, 1) * vehicle_mass  # Load distribution.
     mh_base = {1: 0.75, 2: 0.25}.get(road_type, 0.1)  # Friction coeff.
 
     alpha, beta = 43.398, 5.1549
-    mh = mh_base * (alpha * np.log(engine_max_power) + beta) / 190
+    mh = mh_base * (alpha * np.log(max_power) + beta) / 190
     # * cos(f) for the gradient of the road. Here we consider as 0
 
     return mass * 9.8066 * mh / vehicle_mass
 
 
 @sh.add_function(dsp, outputs=["curves"])
-def calculate_curves_to_use(poly_spline, start, stop, Alimit, car_res_curve, sp_bins):
+def calculate_curves_to_use(
+    poly_spline,
+    poly_spline_electric,
+    start,
+    stop,
+    start_electric,
+    stop_electric,
+    Alimit,
+    car_res_curve,
+    sp_bins,
+    fuel_mode,
+):
     """
     Calculate the final speed acceleration curves based on full load curves and
     resistances for all curves.
 
     :param poly_spline:
         Poly spline.
     :type poly_spline:
@@ -584,25 +772,39 @@
         Final speed and acceleration curves.
     :rtype: list
     """
     from scipy.interpolate import interp1d
 
     res = []
 
-    for gear, acc in enumerate(poly_spline):
+    for gear in range(len(poly_spline)):
         start_ = start[gear] * 0.9
         stop_ = stop[gear] + 0.1
-        if len(poly_spline) == 1:  # for EV
+
+        if fuel_mode == "electric engine":  # for EV
             stop_ = stop[gear]
 
-        final_acc = acc(sp_bins) - car_res_curve(sp_bins)
-        final_acc[final_acc > Alimit] = Alimit
+        motor_1_acc = poly_spline[gear](sp_bins)
+        motor_1_acc[(sp_bins < start_)] = 0
+        motor_1_acc[(sp_bins > stop_)] = 0
+
+        motor_2_acc = 0
+        if fuel_mode == "hybrid":  # for HEV
+            motor_2_acc = poly_spline_electric[gear](sp_bins)
+            motor_2_acc[(sp_bins < start_electric[gear])] = 0
+            motor_2_acc[(sp_bins > stop_electric[gear])] = 0
+
+        tractive_acc = motor_1_acc + motor_2_acc
+        tractive_acc[tractive_acc > Alimit] = Alimit
+        final_acc = tractive_acc - car_res_curve(sp_bins)
+
+        if fuel_mode == "hybrid":
+            phi = 1.035
+            final_acc = final_acc / phi
 
-        final_acc[(sp_bins < start_)] = 0
-        final_acc[(sp_bins > stop_)] = 0
         final_acc[final_acc < 0] = 0
 
         res.append(interp1d(sp_bins, final_acc))
 
     return res
 
 
@@ -622,15 +824,16 @@
     from scipy.interpolate import interp1d
 
     ppar = [0.0045, -0.1710, -1.8835]
     dec_curves = np.poly1d(ppar)
 
     curves_dec = []
     for gear in range(len(stop)):
-        sp_bins = np.arange(0, stop[gear] + 0.1, 0.1)
+        # print(stop)
+        sp_bins = np.arange(0, stop[-1] + 0.1, 0.1)
         final_dec = []
         for k in range(len(sp_bins)):
             final_dec.append(min(dec_curves(sp_bins[k]), -1))
         curves_dec.append(interp1d(sp_bins, final_dec))
 
     return curves_dec
 
@@ -739,15 +942,15 @@
     function=sh.bypass,
     inputs=["idle_engine_speed_median", "idle_engine_speed_std"],
     outputs=["idle_engine_speed"],
 )
 
 
 @sh.add_function(dsp, outputs=["tans"])
-def find_list_of_tans_from_coefs(coefs_per_gear, start, stop):
+def find_list_of_tans_from_coefs(coefs_per_gear, start, stop, fuel_mode):
     """
     Get coefficients and speed boundaries and return Tans value for per speed
     per gear.
 
     :param coefs_per_gear:
         Coefficients per gear.
     :type coefs_per_gear: list
@@ -761,14 +964,17 @@
     :type stop: list
 
     :return:
         Tangential values (derivative of force of each gear with respect to the
         speed).
     :rtype: list
     """
+    if fuel_mode == "electric engine":
+        return sh.NONE
+
     degree = len(coefs_per_gear[0]) - 1
     _vars = np.arange(degree, -1, -1)
 
     tans = []
 
     for gear, coefs in enumerate(coefs_per_gear):
         x_new = np.arange(start[gear], stop[gear], 0.1)
@@ -825,18 +1031,60 @@
 
     gear_cut = tmp_min + i_cut / 10 + 0.1
 
     return gear_cut
 
 
 @sh.add_function(dsp, outputs=["gs"])
-def default_gs(fuel_type):
-    if fuel_type == "electricity":
-        return []
-    return sh.NONE
+def default_gs(
+    motor_speed_per_gear,
+    poly_spline,
+    gear_box_ratios,
+    gear_shifting_style,
+    fuel_type,
+    use_linear_gs=True,
+):
+    if (fuel_type != "electricity") or (not use_linear_gs):
+        return sh.NONE
+
+    ############# This is copied from conventional vehicles
+    # Find where the curve of each gear cuts the next one.
+    for j in range(len(gear_box_ratios) - 1):
+        for k in range(
+            np.minimum(len(motor_speed_per_gear[j]), len(motor_speed_per_gear[j + 1]))
+        ):
+            if (motor_speed_per_gear[j][k] > motor_speed_per_gear[j + 1][0]) & (
+                poly_spline[j + 1](motor_speed_per_gear[j][k])
+                > poly_spline[j](motor_speed_per_gear[j][k])
+            ):
+                max_point = k
+                motor_speed_per_gear[j] = motor_speed_per_gear[j][:max_point]
+                # motor_acc_per_gear[j] = motor_acc_per_gear[j][:max_point]
+                break
+
+    ############# end of copy
+    n_gears = len(motor_speed_per_gear)
+
+    gear_shifting_style = min(gear_shifting_style, 1)
+    gear_shifting_style = max(gear_shifting_style, 0)
+
+    gs = []
+
+    for gear in range(n_gears - 1):
+        speed_by_gs = motor_speed_per_gear[gear][
+            -1
+        ] * gear_shifting_style + motor_speed_per_gear[gear][0] * (
+            1 - gear_shifting_style
+        )
+        speed_for_continuity = motor_speed_per_gear[gear + 1][0]
+        cutoff_s = max(speed_by_gs, speed_for_continuity)
+
+        gs.append(cutoff_s)
+
+    return gs
 
 
 @sh.add_function(dsp, inputs_kwargs=True, outputs=["gs"])
 def gear_points_from_tan(tans, gear_shifting_style, start, use_linear_gs=False):
     """
     Get the gear cuts based on gear shifting style and tangent values.
 
@@ -902,36 +1150,69 @@
     :return:
         Time series.
     :rtype: numpy.array
     """
     return np.arange(sim_start, duration + sim_step, sim_step)
 
 
+# dsp.add_data('engine_max_speed_at_max_power', 0)
+# dsp.add_data('engine_max_power', 0)
+
+
+def empty_full_load_curve_for_electrics(fuel_mode):
+    if fuel_mode != "electric engine":
+        return sh.NONE
+    func = functools.partial(np.interp, xp=[0, 1000], fp=[0, 0], left=0, right=0)
+    return func
+
+
+dsp.add_func(
+    empty_full_load_curve_for_electrics,
+    inputs=["fuel_mode"],
+    outputs=["full_load_curve"],
+)
+
+
+dsp.add_data("engine_max_torque", 0)
+dsp.add_data("fuel_eng_capacity", 0)
+dsp.add_data("fuel_engine_stroke", 0)
+dsp.add_data("drive_battery_voltage", 0)
+dsp.add_data("drive_battery_capacity", 0.000001)
+dsp.add_data("motor_max_power", 0)
+dsp.add_data("engine_max_power", 0)
+dsp.add_data("fuel_turbo", False)
+
+
 @sh.add_function(dsp, outputs=["driver_simulation_model"])
 def define_driver_simulation_model(
     vehicle_mass,
     r_dynamic,
     car_type,
     final_drive_ratio,
     gear_box_ratios,
     gearbox_type,
     engine_max_torque,
     fuel_eng_capacity,
     max_power,
     fuel_engine_stroke,
     fuel_type,
+    fuel_mode,
     fuel_turbo,
     type_of_car,
     car_width,
     car_height,
     transmission,
     gs,
     curves,
     curves_dec,
     driver_style,
+    drive_battery_voltage,
+    drive_battery_capacity,
+    motor_full_load_curve,
+    full_load_curve,
 ):
     """
         Defines the drivers simulation model.
 
     :param vehicle_mass:
         Vehicle mass.
     :type: float
@@ -1014,139 +1295,40 @@
 
     :return:
         Driver simulation model.
     :rtype
     """
     from .driver import Driver
 
-    if fuel_type == "electricity":
-        return sh.NONE
-    return Driver(
-        vehicle_mass,
-        car_type,
-        final_drive_ratio,
-        gearbox_type,
-        max_power,
-        fuel_type,
-        type_of_car,
-        car_width,
-        car_height,
-        transmission,
-        gs,
-        curves,
-        curves_dec,
-        driver_style,
-        r_dynamic,
-        gear_box_ratios,
-        engine_max_torque,
-        fuel_eng_capacity,
-        fuel_engine_stroke,
-        fuel_turbo,
-    )
-
-
-@sh.add_function(dsp, outputs=["driver_simulation_model"])
-def define_ev_driver_simulation_model(
-    vehicle_mass,
-    car_type,
-    final_drive_ratio,
-    gearbox_type,
-    max_power,
-    fuel_type,
-    type_of_car,
-    car_width,
-    car_height,
-    transmission,
-    gs,
-    curves,
-    curves_dec,
-    driver_style,
-):
-    """
-        Defines the drivers simulation model.
-
-    :param vehicle_mass:
-        Vehicle mass.
-    :type: float
-
-    :param car_type:
-        Car type.
-    :type: int
-
-    :param final_drive_ratio:
-        Final drive ratio.
-    :type: float
-
-    :param gearbox_type:
-        Gearbox type.
-    :type: str
-
-    :param max_power:
-        Maximum power.
-    :type: int
-
-    :param fuel_type:
-        Fuel type.
-    :type: str
-
-    :param car_width:
-        Car width.
-    :type: float
-
-    :param car_height:
-        Car height.
-    :type: float
-
-    :param type_of_car:
-        Type of car.
-    :type: str
-
-    :param transmission:
-        Vehicle transmission system.
-    :type: str
-
-    :param gs:
-        Gear cuts.
-    :type: list
-
-    :param curves:
-        Acceleration potential curves per gear.
-    :type: list
-
-    :param curves_dec:
-        Deceleration potential curves per gear.
-    :type: list
-
-    :param driver_style:
-        Driver style.
-    :type: int
-
-    :return:
-        Driver simulation model.
-    :rtype
-    """
-    from .driver import Driver
-
-    if fuel_type != "electricity":
-        return sh.NONE
     return Driver(
         vehicle_mass,
         car_type,
         final_drive_ratio,
         gearbox_type,
         max_power,
         fuel_type,
+        fuel_mode,
         type_of_car,
         car_width,
         car_height,
         transmission,
         gs,
         curves,
         curves_dec,
         driver_style,
+        drive_battery_voltage,
+        drive_battery_capacity,
+        motor_full_load_curve,
+        full_load_curve,
+        r_dynamic=r_dynamic,
+        gear_box_ratios=gear_box_ratios,
+        engine_max_torque=engine_max_torque,
+        fuel_eng_capacity=fuel_eng_capacity,
+        fuel_engine_stroke=fuel_engine_stroke,
+        fuel_turbo=fuel_turbo,
     )
 
 
 @sh.add_function(dsp, outputs=["gears", "gear_counts", "velocities", "accelerations"])
 def run_simulation(
     driver_simulation_model, starting_velocity, sim_step, times, desired_velocity
 ):
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/model/co2mpas.py` & `co2mpas_driver-1.3.3/co2mpas_driver/model/co2mpas.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,51 +2,61 @@
 #
 # Copyright 2019 European Commission (JRC);
 # Licensed under the EUPL (the 'Licence');
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 """
 Functions to process a CO2MPAS input file.
-
-Sub-Modules:
-.. currentmodule:: co2mpas_driver.model.co2mpas
-.. autosummary::
-:nosignatures:
-:toctree: co2mpas/
 """
 
 # Computation of the MFC vehicle acceleration - speed curve.
 # coding=utf-8
 import functools
 import numpy as np
+import schedula as sh
 from scipy.interpolate import CubicSpline
 from co2mpas_driver.common import defaults as defaults
 
 
-def get_full_load(ignition_type):
+def get_full_load(
+    ignition_type,
+    engine_max_speed_at_max_power,
+    engine_max_power,
+    fuel_mode,
+    idle_engine_speed,
+):
     """
     Get vehicle full load curve.
 
     :param ignition_type:
         Engine ignition type (positive or compression).
     :type ignition_type: str
 
     :return:
         Vehicle normalized full load curve.
     :rtype: scipy.interpolate.InterpolatedUnivariateSpline
     """
-
+    if fuel_mode == "electric engine":
+        return sh.NONE
+    #     xp = [0, 0]; fp = [0, 0]
+    # else:
     xp, fp = defaults.dfl.functions.get_full_load.FULL_LOAD[ignition_type]
-    func = functools.partial(np.interp, xp=xp, fp=fp, left=fp[0], right=fp[-1])
+    fp = np.array(fp)
+    fp *= engine_max_power
+    xp = np.array(xp)
+    idle = idle_engine_speed[0]
+    xp = xp * (engine_max_speed_at_max_power - idle) + idle
+
+    func = functools.partial(np.interp, xp=xp, fp=fp, left=0, right=0)
 
     return func
 
 
 def calculate_full_load_speeds_and_powers(
-    full_load_curve, engine_max_power, engine_max_speed_at_max_power, idle_engine_speed
+    full_load_curve, engine_max_speed_at_max_power, idle_engine_speed
 ):
     """
     Calculates the full load speeds and powers [RPM, kW].
 
     :param full_load_curve:
         Vehicle normalized full load curve.
     :type full_load_curve: scipy.interpolate.InterpolatedUnivariateSpline
@@ -63,19 +73,20 @@
         Engine speed idle median and std [RPM].
     :type idle_engine_speed: (float, float)
 
     :return:
          T1 map speed [RPM] and power [kW] vectors.
     :rtype: (numpy.array, numpy.array)
     """
-
+    # if fuel_mode == 'electric engine':
+    #     return np.array([0]), np.array([0])
     n_norm = np.arange(0.0, 1.21, 0.1)
-    full_load_powers = full_load_curve(n_norm) * engine_max_power
     idle = idle_engine_speed[0]
     full_load_speeds = n_norm * (engine_max_speed_at_max_power - idle) + idle
+    full_load_powers = full_load_curve(full_load_speeds)
 
     return full_load_speeds, full_load_powers
 
 
 def calculate_full_load_torques(full_load_speeds, full_load_powers):
     """
     Calculate Full load curves of speed and torque.
@@ -88,14 +99,15 @@
         Engine nominal power [kW].
     :type full_load_speeds: float
 
     :return: full_load_torques
         Full load torques.
     :rtype:
     """
+
     full_load_torques = (
         full_load_powers * 1000 * (full_load_speeds / 60 * 2 * np.pi) ** -1
     )
 
     return full_load_torques
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/model/simulation.py` & `co2mpas_driver-1.3.3/co2mpas_driver/model/simulation.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 """
 Functions to process a CO2MPAS input file.
 """
 
 
-def gear_for_speed_profiles(gs, curr_speed, current_gear, gear_cnt, clutch_duration=5):
+def gear_for_speed_profiles(
+    gs, curr_speed, current_gear, gear_cnt, clutch_duration=5
+):  # ORIGINALLY 5, THEN MAYBE 8
     """
     Return the gear that must be used and the clutch condition.
 
     :param gs:
         Gear limits.
     :type gs: list
 
@@ -65,15 +67,23 @@
                 current_gear = gear_search
                 itr = 0
             else:
                 gear_search += 1
         return current_gear, gear_cnt
 
 
-def accMFC(velocity, driver_style, desired_velocity, acc_p_curve):
+def accMFC(
+    velocity,
+    driver_style,
+    desired_velocity,
+    acc_p_curve,
+    dec_curve,
+    driver_behavior_model="horizontal_b",
+    overshoot=0,
+):
     """
     Calculate the MFC free flow acceleration.
 
     :param velocity:
         speed. (m/s)
     :type velocity: int
 
@@ -87,27 +97,54 @@
 
     :param acc_p_curve:
         Speed acceleration curve of the gear in use.
     :type acc_p_curve:
 
     :return:
     """
-    if velocity / desired_velocity > 0.5:
-        if desired_velocity > velocity:
-            on_off = 1 - pow(velocity / desired_velocity, 60)
+    if driver_behavior_model == "MFC":
+        if velocity / desired_velocity > 0.5:
+            if desired_velocity > velocity:
+                on_off = 1 - pow(velocity / desired_velocity, 60)
+            else:
+                on_off = 10 * (1 - velocity / desired_velocity)
         else:
-            on_off = 10 * (1 - velocity / desired_velocity)
-    else:
-        on_off = 1 - 0.8 * pow(1 - velocity / desired_velocity, 60)
-    acc = acc_p_curve(velocity) * driver_style * on_off
+            on_off = 1 - 0.8 * pow(1 - velocity / desired_velocity, 60)
+
+        if desired_velocity >= velocity:
+            acc = acc_p_curve(velocity) * driver_style * on_off
+        else:
+            acc = dec_curve(velocity) * driver_style * on_off
+    elif driver_behavior_model == "horizontal_a":
+        if velocity >= desired_velocity:
+            on_off = 1 - pow(1 - (velocity - desired_velocity - overshoot) / 50, 100)
+            acc = dec_curve(velocity) * driver_style * on_off
+        elif velocity >= 0.5 * desired_velocity:
+            on_off = 1 - pow(1 + (velocity - desired_velocity - overshoot) / 50, 100)
+            acc = acc_p_curve(velocity) * driver_style * on_off
+        else:
+            on_off = 1 - 0.8 * pow(1 - velocity / (desired_velocity + overshoot), 60)
+            acc = acc_p_curve(velocity) * driver_style * on_off
+    elif driver_behavior_model == "horizontal_b":
+        on_off = max(
+            1
+            - pow(1 + 2 * (velocity - desired_velocity) / (desired_velocity + 0.1), 30),
+            1 - pow(1 - (velocity - desired_velocity) / 50, 100),
+        )
+        if velocity <= desired_velocity:
+            acc = acc_p_curve(velocity) * driver_style * on_off
+        else:
+            acc = dec_curve(velocity) * driver_style * on_off
 
     return acc
 
 
-def correct_acc_clutch_on(gear_count, acc, transmission):
+def correct_acc_clutch_on(
+    gear_count, acc, transmission, automatic_percentage_drop=0.5
+):  # automatic_percentage_drop=2/3
     """
     Get the acceleration If clutch is on. Maximum acceleration is
     decreased depending on the transmission.
 
     :param gear_count:
         Gear count.
     :type gear_count: int
@@ -122,14 +159,13 @@
 
     :return:
         Acceleration when clutch on. (m/s2)
     :rtype:
     """
 
     if gear_count > 0:
-
         if transmission == "manual":
             return 0.0
         else:
-            return acc * 2 / 3
+            return acc * automatic_percentage_drop
     else:
         return acc
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/plot.py` & `co2mpas_driver-1.3.3/co2mpas_driver/plot.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/sample_simulation.py` & `co2mpas_driver-1.3.3/co2mpas_driver/sample_simulation.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver/template/sample.xlsx` & `co2mpas_driver-1.3.3/co2mpas_driver/template/sample.xlsx`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver.egg-info/PKG-INFO` & `co2mpas_driver-1.3.3/co2mpas_driver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: co2mpas-driver
-Version: 1.3.1
+Version: 1.3.3
 Summary: A lightweight microsimulation free-flow acceleration model(MFC) or co2mpas_driver is a model that is able to capture the vehicle acceleration dynamics accurately and consistently
 License: European Union Public Licence 1.1 or later (EUPL 1.1+)
-Project-URL: Sources, https://github.com/JRCSTU/co2mpas_driver
+Project-URL: Sources, https://code.europa.eu/jrc-ldv/co2mpas_driver
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -16,22 +16,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
-.. figure:: ./co2mpas_driver/images/co2mpas_driver_logo.png
-    :align: center
-    :alt: alternate text
-    :figclass: align-center
+|JRC-image|
 
 .. _start-info:
 
 
 :versions:      |gh-version| |rel-date| |python-ver|
 :documentation: https://co2mpas-driver.readthedocs.io/en/latest/
 :sources:       https://code.europa.eu/jrc-ldv/co2mpas-driver |pypi-ins| |codestyle|
@@ -129,16 +125,17 @@
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
 
 * *co2mpas_driver* must be imported as a dispatcher (dsp). The dsp contains
   functions to process vehicle data and run the *com2pas_driver* model. Also is necessary
   to import *schedula* for selecting and executing functions from the *co2mpas_driver*.
   For more information on how to use *schedula*: https://pypi.org/project/schedula/
-      >>> from co2mpas_driver import dsp
-      >>> import schedula as sh
+  
+        >>> from co2mpas_driver import dsp
+        >>> import schedula as sh
 
 Load data
 ---------
 * Load vehicle data for a specific vehicle from vehicles database
 
         >>> db_path = 'EuroSegmentCar.csv'
 
@@ -281,19 +278,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitHub%20-1.3.1-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2022/10/14-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -307,14 +304,19 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.0-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
+.. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
+    :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
+    :alt: GitLab repository
+
+
 .. |CO2| replace:: CO\ :sub:`2`
 
 .. _end-sub:
```

### Comparing `co2mpas_driver-1.3.1/co2mpas_driver.egg-info/SOURCES.txt` & `co2mpas_driver-1.3.3/co2mpas_driver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 co2mpas_driver/common/reading_n_organizing.py
 co2mpas_driver/common/simulation_part.py
 co2mpas_driver/common/utils.py
 co2mpas_driver/common/vehicle_functions.py
 co2mpas_driver/common/vehicle_specs_class.py
 co2mpas_driver/db/EuroSegmentCar.csv
 co2mpas_driver/db/EuroSegmentCar_cleaned.csv
+co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv
 co2mpas_driver/examples/Sim_Kat_for_Jaime_2.py
 co2mpas_driver/examples/__init__.py
+co2mpas_driver/examples/calculate_on_existing_example.py
+co2mpas_driver/examples/mfc_post_proc_trajectory.py
 co2mpas_driver/examples/new_test.py
 co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py
 co2mpas_driver/examples/sample_gear_shifting.py
 co2mpas_driver/examples/sample_light_co2mpas.py
 co2mpas_driver/examples/sample_simulation.py
 co2mpas_driver/examples/sample_varying_des_speed.py
+co2mpas_driver/examples/sample_varying_des_speed_yl_2.py
 co2mpas_driver/examples/sample_veh_specs_collection.py
 co2mpas_driver/examples/test.py
 co2mpas_driver/model/__init__.py
 co2mpas_driver/model/co2mpas.py
 co2mpas_driver/model/driver.py
 co2mpas_driver/model/simulation.py
 co2mpas_driver/template/sample.xlsx
```

### Comparing `co2mpas_driver-1.3.1/model_validation/test_core.py` & `co2mpas_driver-1.3.3/model_validation/test_core.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/model_validation/utils.py` & `co2mpas_driver-1.3.3/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.1/setup.py` & `co2mpas_driver-1.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,49 +15,49 @@
 from os import path as osp
 
 my_dir = osp.dirname(osp.abspath(__file__))
 os.chdir(my_dir)
 
 name = "co2mpas_driver"
 
+
 if __name__ == "__main__":
     from setuptools import setup, find_packages
 
+    def read_file(fpath):
+        with open(fpath) as fd:
+            return fd.read()
+
     dir_list = ["build", "dist", "{}.egg-info".format(name)]
 
     for d in dir_list:
         try:
             shutil.rmtree(d)
         except:
             pass
 
-    def readme():
-        with open("README.rst") as f:
-            return f.read()
-
     test_deps = ["pytest"]
 
-    url = "https://github.com/JRCSTU/%s" % name
+    url = "https://code.europa.eu/jrc-ldv/%s" % name
 
     setup(
         name=name,
-        version="1.3.1",
+        version="1.3.3",
         packages=find_packages(
             exclude=[
                 "test",
                 "test.*",
             ]
         ),
         license="European Union Public Licence 1.1 or later (EUPL 1.1+)",
         description="A lightweight microsimulation free-flow acceleration model"
         "(MFC) or co2mpas_driver is a model that is able to "
         "capture the vehicle acceleration dynamics accurately and "
         "consistently",
-        long_description=readme(),
-        long_description_content_type="text/markdown",
+        long_description=read_file("README.rst"),
         project_urls={"Sources": url},
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Intended Audience :: Science/Research",
             "Intended Audience :: Manufacturing",
             "Programming Language :: Python :: 3",
@@ -70,24 +70,26 @@
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: POSIX",
             "Operating System :: Unix",
         ],
         install_requires=[
             "PyYAML",
-            "schedula>=0.3.2",
+            "schedula[all]>=0.3.2",
             "tqdm",
             "scikit-learn",
             "regex",
             "lmfit>=0.9.7",
             "numpy",
             "schema",
             "scipy",
             "wltp",
             "xgboost",
+            "pandas",
+            "networkx",
         ],
         tests_require=test_deps,
         package_data={"co2mpas_driver": ["template/*.xlsx", "db/*.csv", "*"]},
         entry_points="""[console_scripts]
         run_simulation=co2mpas_driver.sample_simulation:run_simulation""",
         include_package_data=True,
         zip_safe=True,
```


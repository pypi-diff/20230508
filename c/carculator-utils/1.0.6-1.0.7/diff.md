# Comparing `tmp/carculator_utils-1.0.6.tar.gz` & `tmp/carculator_utils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator_utils-1.0.6.tar", last modified: Wed Apr 26 07:25:09 2023, max compression
+gzip compressed data, was "carculator_utils-1.0.7.tar", last modified: Mon May  8 14:29:51 2023, max compression
```

## Comparing `carculator_utils-1.0.6.tar` & `carculator_utils-1.0.7.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/background_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.203723 carculator_utils-1.0.6/carculator_utils/data/IAM/
--rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/A_matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/driving cycle/
--rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/dc_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/efficiency/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/car.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/truck.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/electricity/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/cumulative_electricity_losses.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/elec_tech_map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/electricity_mixes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/
--rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/euro_classes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/noise_flows.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.211723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.211723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei35.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei36.csv
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei38_to_ei37.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154654 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/references.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/rename_parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/rename_powertrains.yml
--rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro-biosphere.json
--rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro-technosphere-3.5.csv
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro_blacklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro_fields.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/fuel/
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/S_concentration_fuel.csv
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/default_fuels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/fuel_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_cng.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_diesel.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_gasoline.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/gradient/
--rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/lcia/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/lcia/dict_impact_categories.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/lcia/impact_source_categories.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/monthly_avg_temp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/purchase_cost_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/driving_cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23683 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    42445 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/hot_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    51873 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/noise_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/particulates_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/vehicle_input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/tests/test_vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.000215 carculator_utils-1.0.7/carculator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/background_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.000215 carculator_utils-1.0.7/carculator_utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.032214 carculator_utils-1.0.7/carculator_utils/data/IAM/
+-rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/A_matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/driving cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/driving cycle/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/driving cycle/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/driving cycle/dc_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/driving cycle/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/driving cycle/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/efficiency/bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/efficiency/car.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/efficiency/truck.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/electricity/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/electricity/cumulative_electricity_losses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/electricity/elec_tech_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/electricity/electricity_mixes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/emission_factors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.036214 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/euro_classes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/exhaust_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/noise_flows.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.040214 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.040214 carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.044214 carculator_utils-1.0.7/carculator_utils/data/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/ei37_to_ei35.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/ei37_to_ei36.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/ei38_to_ei37.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154843 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/references.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/rename_parameters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/rename_powertrains.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/simapro-biosphere.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/simapro-technosphere-3.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/simapro_blacklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/export/simapro_fields.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/carculator_utils/data/fuel/
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/S_concentration_fuel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/default_fuels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/fuel_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_cng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_diesel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_gasoline.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/carculator_utils/data/gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/gradient/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/gradient/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/gradient/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/gradient/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/carculator_utils/data/lcia/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/lcia/dict_impact_categories.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/lcia/impact_source_categories.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/monthly_avg_temp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/data/purchase_cost_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/driving_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23683 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42445 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/hot_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68164 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51709 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/noise_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/particulates_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/carculator_utils/vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.000215 carculator_utils-1.0.7/carculator_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-08 14:29:50.000000 carculator_utils-1.0.7/carculator_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-08 14:29:50.000000 carculator_utils-1.0.7/carculator_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:29:50.000000 carculator_utils-1.0.7/carculator_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 14:29:50.000000 carculator_utils-1.0.7/carculator_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 14:29:50.000000 carculator_utils-1.0.7/carculator_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:29:51.048214 carculator_utils-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 14:29:43.000000 carculator_utils-1.0.7/tests/test_vehicle_input_parameters.py
```

### Comparing `carculator_utils-1.0.6/CODE_OF_CONDUCT.md` & `carculator_utils-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/CONTRIBUTING.md` & `carculator_utils-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/LICENSE` & `carculator_utils-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/PKG-INFO` & `carculator_utils-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator_utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

### Comparing `carculator_utils-1.0.6/README.md` & `carculator_utils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/__init__.py` & `carculator_utils-1.0.7/carculator_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "NoiseEmissionsModel",
     "HotEmissionsModel",
     "Inventory",
     "BackgroundSystemModel",
     "ExportInventory",
     "VehicleInputParameters",
 )
-__version__ = (1, 0, 6)
+__version__ = (1, 0, 7)
 
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 from .background_systems import BackgroundSystemModel
 from .driving_cycles import get_standard_driving_cycle_and_gradient
```

### Comparing `carculator_utils-1.0.6/carculator_utils/array.py` & `carculator_utils-1.0.7/carculator_utils/array.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/background_systems.py` & `carculator_utils-1.0.7/carculator_utils/background_systems.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/A_matrix.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/IAM/dict_inputs_A_matrix.csv` & `carculator_utils-1.0.7/carculator_utils/data/IAM/dict_inputs_A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/driving cycle/bus.csv` & `carculator_utils-1.0.7/carculator_utils/data/driving cycle/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/driving cycle/car.csv` & `carculator_utils-1.0.7/carculator_utils/data/driving cycle/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/driving cycle/dc_specs.yaml` & `carculator_utils-1.0.7/carculator_utils/data/driving cycle/dc_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/driving cycle/truck.csv` & `carculator_utils-1.0.7/carculator_utils/data/driving cycle/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/driving cycle/two-wheeler.csv` & `carculator_utils-1.0.7/carculator_utils/data/driving cycle/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/efficiency/bus.yaml` & `carculator_utils-1.0.7/carculator_utils/data/efficiency/bus.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/efficiency/car.yaml` & `carculator_utils-1.0.7/carculator_utils/data/efficiency/car.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/efficiency/truck.yaml` & `carculator_utils-1.0.7/carculator_utils/data/efficiency/truck.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/electricity/cumulative_electricity_losses.csv` & `carculator_utils-1.0.7/carculator_utils/data/electricity/cumulative_electricity_losses.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/electricity/elec_tech_map.yaml` & `carculator_utils-1.0.7/carculator_utils/data/electricity/elec_tech_map.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/electricity/electricity_mixes.csv` & `carculator_utils-1.0.7/carculator_utils/data/electricity/electricity_mixes.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/NMHC_species.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/NMHC_species.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/degradation_EF.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/degradation_EF.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/engine_wear.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/car/engine_wear.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/euro_classes.yaml` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/euro_classes.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_flows.yaml` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/exhaust_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/noise_flows.yaml` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.7/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei35.csv` & `carculator_utils-1.0.7/carculator_utils/data/export/ei37_to_ei35.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei36.csv` & `carculator_utils-1.0.7/carculator_utils/data/export/ei37_to_ei36.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/ei38_to_ei37.csv` & `carculator_utils-1.0.7/carculator_utils/data/export/ei38_to_ei37.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/references.csv` & `carculator_utils-1.0.7/carculator_utils/data/export/references.csv`

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,9 @@
 gearbox, for lorry;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of gearbox for a MDV/HDV.;;transport;Road\Vehicle components
 frame, blanks and saddle, for lorry;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of frame, blanks and saddle for a MDV/HDV.;;transport;Road\Vehicle components
 exhaust system, for lorry;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of exhaust system for a MDV/HDV.;;transport;Road\Vehicle components
 cabin, for lorry;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of cabin for a MDV/HDV.;;transport;Road\Vehicle components
 assembly operation, for lorry;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of cabin for a MDV/HDV.;;transport;Road\Vehicle components
 fuel tank, for diesel vehicle;Wolff et al. 2020, Sustainability, DOI: 10.3390/su12135396;This is the inventory for 1 kg of aluminium-made fuel tank, empty. Scaling formula: 17.159*ln(volume fuel)-54.98;;transport;Road\Vehicle components
 electric bicycle production, without battery and motor;ecoinvent 3.8;Electric bicycle production, without the battery and the electric motor.;;transport;Road\Vehicle components
+electric cargo bicycle production, without battery and motor;ecoinvent 3.8;Electric cargo bicycle production, without the battery and the electric motor.;;transport;Road\Vehicle components
 maintenance, electric bicycle, without battery;ecoinvent 3.8;Electric bicycle production, without the battery and the electric motor.;;transport;Road\Vehicle components
```

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/rename_parameters.yml` & `carculator_utils-1.0.7/carculator_utils/data/export/rename_parameters.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/simapro-biosphere.json` & `carculator_utils-1.0.7/carculator_utils/data/export/simapro-biosphere.json`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/simapro-technosphere-3.5.csv` & `carculator_utils-1.0.7/carculator_utils/data/export/simapro-technosphere-3.5.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/export/simapro_fields.yml` & `carculator_utils-1.0.7/carculator_utils/data/export/simapro_fields.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/S_concentration_fuel.csv` & `carculator_utils-1.0.7/carculator_utils/data/fuel/S_concentration_fuel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/default_fuels.yaml` & `carculator_utils-1.0.7/carculator_utils/data/fuel/default_fuels.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/fuel_specs.yaml` & `carculator_utils-1.0.7/carculator_utils/data/fuel/fuel_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_cng.csv` & `carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_cng.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_diesel.csv` & `carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_diesel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_gasoline.csv` & `carculator_utils-1.0.7/carculator_utils/data/fuel/share_bio_gasoline.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/gradient/bus.csv` & `carculator_utils-1.0.7/carculator_utils/data/gradient/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/gradient/car.csv` & `carculator_utils-1.0.7/carculator_utils/data/gradient/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/gradient/truck.csv` & `carculator_utils-1.0.7/carculator_utils/data/gradient/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/gradient/two-wheeler.csv` & `carculator_utils-1.0.7/carculator_utils/data/gradient/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/lcia/dict_impact_categories.csv` & `carculator_utils-1.0.7/carculator_utils/data/lcia/dict_impact_categories.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/lcia/impact_source_categories.yml` & `carculator_utils-1.0.7/carculator_utils/data/lcia/impact_source_categories.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/monthly_avg_temp.csv` & `carculator_utils-1.0.7/carculator_utils/data/monthly_avg_temp.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/data/purchase_cost_params.yaml` & `carculator_utils-1.0.7/carculator_utils/data/purchase_cost_params.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/driving_cycles.py` & `carculator_utils-1.0.7/carculator_utils/driving_cycles.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/energy_consumption.py` & `carculator_utils-1.0.7/carculator_utils/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/export.py` & `carculator_utils-1.0.7/carculator_utils/export.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/hot_emissions.py` & `carculator_utils-1.0.7/carculator_utils/hot_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/inventory.py` & `carculator_utils-1.0.7/carculator_utils/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1297,17 +1297,14 @@
             self.find_input_indices((f"Battery cell, {battery_tech[0]}",)),
             self.find_input_indices((f"{self.vm.vehicle_type.capitalize()}, ",)),
         ] = (
             self.array[self.array_inputs["battery cell mass"], :]
             * (1 + self.array[self.array_inputs["battery lifetime replacements"], :])
         ) * -1
 
-        # Set an input of electricity, given the country of manufacture
-        print(f"Battery cell, {battery_tech[0]}")
-
         electricity_batt = self.find_input_requirement(
             value_in="kilowatt hour",
             value_out=f"Battery cell, {battery_tech[0]}",
             find_input_by="unit",
             filter_activities=["NMC", "LFP", "LTO", "NCA"],
             zero_out_input=True,
         )
```

### Comparing `carculator_utils-1.0.6/carculator_utils/model.py` & `carculator_utils-1.0.7/carculator_utils/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         country="CH",
         cycle: Union[None, str, np.ndarray] = None,
         gradient: Union[None, np.ndarray] = None,
         energy_storage: Union[None, Dict] = None,
         electric_utility_factor: float = None,
         drop_hybrids: bool = True,
         payload=None,
+        annual_mileage=None,
         energy_target=None,
         energy_consumption: dict = None,
         target_range: dict = None,
         target_mass: dict = None,
         power: dict = None,
         fuel_blend: dict = None,
         ambient_temperature: float = None,
@@ -78,14 +79,15 @@
             else get_default_driving_cycle_name(self.vehicle_type)
         )
 
         self.gradient = gradient
         self.energy_storage = energy_storage or {}
         self.energy_target = energy_target or {2025: 0.85, 2030: 0.7, 2050: 0.6}
         self.payload = payload or {}
+        self.annual_mileage = annual_mileage or {}
 
         self.set_battery_chemistry()
         self.set_battery_preferences()
         self.energy = None
         self.electric_utility_factor = electric_utility_factor
         self.drop_hybrids = drop_hybrids
         self.energy_consumption = energy_consumption or None
@@ -378,14 +380,26 @@
                             powertrain=pwt,
                             size=size,
                             year=year,
                             parameter=["auxiliary energy", "recuperated energy"],
                         )
                     ] = 0
 
+                    # update self["TtW energy"]
+                    self["TtW energy"] = (
+                        self.energy.sel(
+                            parameter=[
+                                "motive energy",
+                                "auxiliary energy",
+                                "recuperated energy",
+                            ]
+                        ).sum(dim=["second", "parameter"])
+                        / distance
+                    ).T
+
     def calculate_ttw_energy(self) -> None:
         """
         This method calculates the energy required to operate auxiliary
         services as well as to move the car. The sum is stored under the
         parameter label "TtW energy" in :attr:`self.array`.
 
         """
@@ -649,17 +663,18 @@
         Calculate the share of recuperated energy,
         over the total negative motive energy.
         """
 
         _ = lambda x: np.where(x == 0, 1, x)
 
         self["share recuperated energy"] = (
-            _(self.energy.sel(parameter="recuperated energy").sum(dim="second"))
+            self.energy.sel(parameter="recuperated energy").sum(dim="second")
             / _(self.energy.sel(parameter="negative motive energy").sum(dim="second"))
-        ).T * (self["combustion power share"] < 1)
+        ).values.T
+        self["share recuperated energy"] *= self["combustion power share"] < 1
 
         if "PHEV-d" in self.array.powertrain:
             self.array.loc[
                 dict(powertrain="PHEV-c-d", parameter="share recuperated energy")
             ] = self.array.loc[
                 dict(powertrain="PHEV-e", parameter="share recuperated energy")
             ]
@@ -976,63 +991,60 @@
             / self["TtW energy"]
         )
 
     def check_fuel_blend(self, fuel_blend: dict) -> dict:
         for fuel, specs in fuel_blend.items():
             if "primary" not in specs:
                 raise ValueError(f"Primary fuel not specified for {fuel}")
-            else:
-                if "share" not in specs["primary"]:
-                    raise ValueError(f"Primary fuel share not specified for {fuel}")
-                else:
-                    if not isinstance(specs["primary"]["share"], np.ndarray):
-                        specs["primary"]["share"] = np.array(specs["primary"]["share"])
-                if "type" not in specs["primary"]:
-                    raise ValueError(f"Primary fuel type not specified for {fuel}")
-                if "name" not in specs["primary"]:
-                    specs["primary"]["name"] = tuple(
-                        self.bs.fuel_specs[specs["primary"]["type"]]["name"]
-                    )
-                if "CO2" not in specs["primary"]:
-                    specs["primary"]["CO2"] = self.bs.fuel_specs[
-                        specs["primary"]["type"]
-                    ]["co2"]
-                if "biogenic share" not in specs["primary"]:
-                    specs["primary"]["biogenic share"] = self.bs.fuel_specs[
-                        specs["primary"]["type"]
-                    ]["biogenic_share"]
-
-            if "secondary" not in specs:
-                specs["secondary"] = {
-                    "type": specs["primary"]["type"],
-                    "share": np.array([1]) - specs["primary"]["share"],
-                }
-            else:
-                if "share" not in specs["secondary"]:
-                    raise ValueError(f"Secondary fuel share not specified for {fuel}")
-                else:
-                    if not isinstance(specs["secondary"]["share"], np.ndarray):
-                        specs["secondary"]["share"] = np.array(
-                            specs["secondary"]["share"]
-                        )
 
-                if "type" not in specs["secondary"]:
-                    raise ValueError(f"Secondary fuel type not specified for {fuel}")
-                if "name" not in specs["secondary"]:
-                    specs["secondary"]["name"] = tuple(
-                        self.bs.fuel_specs[specs["secondary"]["type"]]["name"]
-                    )
-                if "CO2" not in specs["secondary"]:
-                    specs["secondary"]["CO2"] = self.bs.fuel_specs[
-                        specs["secondary"]["type"]
-                    ]["co2"]
-                if "biogenic share" not in specs["secondary"]:
-                    specs["secondary"]["biogenic share"] = self.bs.fuel_specs[
-                        specs["secondary"]["type"]
-                    ]["biogenic_share"]
+            primary = specs["primary"]
+
+            if "share" not in primary:
+                raise ValueError(f"Primary fuel share not specified for {fuel}")
+
+            if not isinstance(primary["share"], np.ndarray):
+                primary["share"] = np.array(primary["share"])
+
+            if "type" not in primary:
+                raise ValueError(f"Primary fuel type not specified for {fuel}")
+
+            primary.setdefault(
+                "name", tuple(self.bs.fuel_specs[primary["type"]]["name"])
+            )
+            primary.setdefault("CO2", self.bs.fuel_specs[primary["type"]]["co2"])
+            primary.setdefault(
+                "biogenic share", self.bs.fuel_specs[primary["type"]]["biogenic_share"]
+            )
+
+            secondary = specs.get(
+                "secondary",
+                {
+                    "type": primary["type"],
+                    "share": np.array([1]) - primary["share"],
+                },
+            )
+            specs["secondary"] = secondary
+
+            if "share" not in secondary:
+                raise ValueError(f"Secondary fuel share not specified for {fuel}")
+
+            if not isinstance(secondary["share"], np.ndarray):
+                secondary["share"] = np.array(secondary["share"])
+
+            if "type" not in secondary:
+                raise ValueError(f"Secondary fuel type not specified for {fuel}")
+
+            secondary.setdefault(
+                "name", tuple(self.bs.fuel_specs[secondary["type"]]["name"])
+            )
+            secondary.setdefault("CO2", self.bs.fuel_specs[secondary["type"]]["co2"])
+            secondary.setdefault(
+                "biogenic share",
+                self.bs.fuel_specs[secondary["type"]]["biogenic_share"],
+            )
 
         return fuel_blend
 
     def set_average_lhv(self) -> None:
         """
         Calculate average LHV of fuel.
         :return:
@@ -1318,21 +1330,21 @@
         ).sum(dim="parameter")
 
         hot_emissions = hem.get_hot_emissions(
             euro_class=list_euro_classes,
             lifetime_km=self["lifetime kilometers"],
             energy_consumption=energy_consumption,
             yearly_km=self["kilometers per year"],
-        )
+        ).values
 
         self.array.loc[
             dict(
                 parameter=list_direct_emissions,
             )
-        ] = hot_emissions.values
+        ] = hot_emissions
 
     def set_particulates_emission(self) -> None:
         """
         Calculate the emission of particulates according to
         https://www.eea.europa.eu/ds_resolveuid/6USNA27I4D
 
         and further disaggregated in:
```

### Comparing `carculator_utils-1.0.6/carculator_utils/noise_emissions.py` & `carculator_utils-1.0.7/carculator_utils/noise_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/particulates_emissions.py` & `carculator_utils-1.0.7/carculator_utils/particulates_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils/vehicle_input_parameters.py` & `carculator_utils-1.0.7/carculator_utils/vehicle_input_parameters.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/carculator_utils.egg-info/PKG-INFO` & `carculator_utils-1.0.7/carculator_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator-utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

### Comparing `carculator_utils-1.0.6/carculator_utils.egg-info/SOURCES.txt` & `carculator_utils-1.0.7/carculator_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/readthedocs.yml` & `carculator_utils-1.0.7/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.6/setup.py` & `carculator_utils-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="carculator_utils",
-    version="1.0.6",
+    version="1.0.7",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     python_requires=">=3.9",
     license=open("LICENSE").read(),
     package_data={
         "carculator_utils": package_files(os.path.join("carculator_utils", "data"))
     },
```

### Comparing `carculator_utils-1.0.6/tests/test_vehicle_input_parameters.py` & `carculator_utils-1.0.7/tests/test_vehicle_input_parameters.py`

 * *Files identical despite different names*


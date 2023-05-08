# Comparing `tmp/carculator_truck-0.3.8.tar.gz` & `tmp/carculator_truck-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator_truck-0.3.8.tar", last modified: Mon Oct 17 09:38:41 2022, max compression
+gzip compressed data, was "carculator_truck-0.3.9.tar", last modified: Mon May  8 16:35:35 2023, max compression
```

## Comparing `carculator_truck-0.3.8.tar` & `carculator_truck-0.3.9.tar`

### file list

```diff
@@ -1,123 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:41.924365 carculator_truck-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-10-17 09:38:41.924365 carculator_truck-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:41.884366 carculator_truck-0.3.8/carculator_truck/
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16986 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/array.py
--rw-r--r--   0 runner    (1001) docker     (121)     7314 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/background_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:41.896366 carculator_truck-0.3.8/carculator_truck/data/
--rw-r--r--   0 runner    (1001) docker     (121)    66701 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/A_matrix_trucks.csv
--rw-r--r--   0 runner    (1001) docker     (121)   137728 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/HEM_factors_trucks.xls
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:41.920365 carculator_truck-0.3.8/carculator_truck/data/IAM/
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   515704 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_ilcd_midpoint_trucks_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108544 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108544 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108544 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108545 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   108541 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_endpoint_trucks_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624602 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624602 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624604 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624603 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624606 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (121)   624601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/IAM/B_matrix_recipe_midpoint_trucks_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14500 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/S_concentration_fuel.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14601 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/biofuel_share.csv
--rw-r--r--   0 runner    (1001) docker     (121)     5650 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/cumulative_electricity_losses.csv
--rw-r--r--   0 runner    (1001) docker     (121)  1456247 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)     6343 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/dict_impact_categories.csv
--rw-r--r--   0 runner    (1001) docker     (121)    81211 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/dict_inputs_A_matrix_trucks.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/dict_split.csv
--rw-r--r--   0 runner    (1001) docker     (121)   392181 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/driving_cycles.csv
--rw-r--r--   0 runner    (1001) docker     (121)     7166 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/ei37_to_ei35.csv
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/ei37_to_ei36.csv
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/ei38_to_ei37.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/elec_tech_map.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/electricity_markets.csv
--rw-r--r--   0 runner    (1001) docker     (121)    98611 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/electricity_mixes.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/exhaust_and_noise_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9895 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/extra_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)     6577 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/fuel_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   764385 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/gradients.csv
--rw-r--r--   0 runner    (1001) docker     (121)    37376 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/hbefa_factors_vs_fc.xls
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/hot_trucks.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/hot_trucks.pickle
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/noise_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/payloads.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   150125 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/references.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/region_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6060 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/regionmappingH12.csv
--rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/share_bio_cng.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14783 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/share_bio_diesel.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14607 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/share_bio_gasoline.csv
--rw-r--r--   0 runner    (1001) docker     (121)    57472 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/simapro-biosphere.json
--rw-r--r--   0 runner    (1001) docker     (121)  6503006 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/simapro-technosphere-3.5.csv
--rw-r--r--   0 runner    (1001) docker     (121)    15537 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/tags.csv
--rw-r--r--   0 runner    (1001) docker     (121)    16683 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/transport_distance_uvek.csv
--rw-r--r--   0 runner    (1001) docker     (121)   110933 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/data/uvek_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/driving_cycles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8972 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (121)    95735 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/geomap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/gradients.py
--rw-r--r--   0 runner    (1001) docker     (121)    10602 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/hot_emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)   192143 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)    87098 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/noise_emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5797 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/particulates_emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/truck_input_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/carculator_truck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:41.884366 carculator_truck-0.3.8/carculator_truck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-10-17 09:38:41.000000 carculator_truck-0.3.8/carculator_truck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7200 2022-10-17 09:38:41.000000 carculator_truck-0.3.8/carculator_truck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 09:38:41.000000 carculator_truck-0.3.8/carculator_truck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-17 09:38:41.000000 carculator_truck-0.3.8/carculator_truck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-17 09:38:41.000000 carculator_truck-0.3.8/carculator_truck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-17 09:38:41.924365 carculator_truck-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-17 09:38:31.000000 carculator_truck-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.810892 carculator_truck-0.3.9/carculator_truck/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/background_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/carculator_truck/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1445083 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/extra_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/payloads.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/driving_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35059 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/truck_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.810892 carculator_truck-0.3.9/carculator_truck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/tests/test_model.py
```

### Comparing `carculator_truck-0.3.8/LICENSE` & `carculator_truck-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.8/PKG-INFO` & `carculator_truck-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator_truck
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prospective environmental and economic life cycle assessmentof medium and heavy goods vehicles
 Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -51,15 +51,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ``carculator_truck``
 
 <p align="center">
-  <img style="height:130px;" src="https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png">
+  <img style="height:130px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/mediumsmall.png">
 </p>
 
 
 <p align="center">
   <a href="https://badge.fury.io/py/carculator-truck" target="_blank"><img src="https://badge.fury.io/py/carculator-truck.svg"></a>
   <a href="https://github.com/romainsacchi/carculator_truck" target="_blank"><img src="https://github.com/romainsacchi/carculator_truck/actions/workflows/main.yml/badge.svg?branch=master"></a>
   <a href="https://coveralls.io/github/romainsacchi/carculator_truck" target="_blank"><img src="https://coveralls.io/repos/github/romainsacchi/carculator_truck/badge.svg"></a>
@@ -105,33 +105,37 @@
 <a href="https://www.simapro.com/" target="_blank">SimaPro 9.x.</a>.</li>
 </ul>
 
 <p align="center">
     The energy model of <i>carculator_truck</i> considers the vehicle aerodynamics, the road gradient and other factors.
     It also considers varying efficiencies of the transmission and engine at various load points for each second
     of the driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/energy_model.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/energy_model.png">
 </p>
 
 <p align="center">
     The energy model and the calculated tank-to-wheel energy consumption is validated against the simulation software
     <a href="https://ec.europa.eu/clima/policies/transport/vehicles/vecto_en" target="_blank">VECTO</a>.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/vecto_validation.png">
 </p>
 
 <p align="center">
     Benefits of hybrid powertrains are fully conidered: the possibility to recuperate braking energy as well as efficiency gains from engine
     downsizing is accounted for.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/hybrid_efficiency.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/hybrid_efficiency.png">
 </p>
 
 <p align="center">
     Global warming potential impacts per ton-km for a 40-t truck, across different powertrain technologies,
     using an urban driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png">
 </p>
 
 ## How to use it?
 
 See the notebook with [examples](https://github.com/romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb).
 
 ## Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator_truck Version: 0.3.8 Summary:
+Metadata-Version: 2.1 Name: carculator_truck Version: 0.3.9 Summary:
 Prospective environmental and economic life cycle assessmentof medium and heavy
 goods vehicles Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi
 sacchi@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
@@ -30,15 +30,16 @@
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Mathematics Classifier: Topic :: Scientific/Engineering ::
 Visualization Description-Content-Type: text/markdown License-File: LICENSE #
 ``carculator_truck``
-   [https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png]
+[https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                               mediumsmall.png]
      [https://badge.fury.io/py/carculator-truck.svg] [https://github.com/
            romainsacchi/carculator_truck/actions/workflows/main.yml/
    badge.svg?branch=master] [https://coveralls.io/repos/github/romainsacchi/
 carculator_truck/badge.svg] [https://readthedocs.org/projects/carculator_truck/
                             badge/?version=latest]
 Prospective environmental and economic life cycle assessment of medium and
 heavy duty vehicles. A fully parameterized Python model developed by the
@@ -67,26 +68,27 @@
       level but also in the rest of the world energy system (e.g., power
       generation) is accounted for, using energy scenario-specific IAM-coupled
       ecoinvent databases produced by premise.
     * Inventories can be imported into Brightway2 and SimaPro_9.x..
  The energy model of carculator_truck considers the vehicle aerodynamics, the
 road gradient and other factors. It also considers varying efficiencies of the
  transmission and engine at various load points for each second of the driving
-   cycle. [https://github.com/romainsacchi/carculator_truck/raw/master/docs/
-                               energy_model.png]
+  cycle. [https://github.com/romainsacchi/carculator_truck/blob/master/docs/
+                         _static/img/energy_model.png]
     The energy model and the calculated tank-to-wheel energy consumption is
      validated against the simulation software VECTO. [https://github.com/
-      romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png]
+          romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                             vecto_validation.png]
     Benefits of hybrid powertrains are fully conidered: the possibility to
 recuperate braking energy as well as efficiency gains from engine downsizing is
- accounted for. [https://github.com/romainsacchi/carculator_truck/raw/master/
-                          docs/hybrid_efficiency.png]
+ accounted for. [https://github.com/romainsacchi/carculator_truck/blob/master/
+                    docs/_static/img/hybrid_efficiency.png]
 Global warming potential impacts per ton-km for a 40-t truck, across different
   powertrain technologies, using an urban driving cycle. [https://github.com/
-         romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png]
+   romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png]
 ## How to use it? See the notebook with [examples](https://github.com/
 romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb). ## Support
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:
 carculator@psi.ch). ## Maintainers * [Romain Sacchi](https://github.com/
 romainsacchi) * [Chris Mutel](https://github.com/cmutel/) ## Contributing See
 [contributing](https://github.com/romainsacchi/carculator_truck/blob/master/
 CONTRIBUTING.md). ## License [BSD-3-Clause](https://github.com/romainsacchi/
```

### Comparing `carculator_truck-0.3.8/README.md` & `carculator_truck-0.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ``carculator_truck``
 
 <p align="center">
-  <img style="height:130px;" src="https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png">
+  <img style="height:130px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/mediumsmall.png">
 </p>
 
 
 <p align="center">
   <a href="https://badge.fury.io/py/carculator-truck" target="_blank"><img src="https://badge.fury.io/py/carculator-truck.svg"></a>
   <a href="https://github.com/romainsacchi/carculator_truck" target="_blank"><img src="https://github.com/romainsacchi/carculator_truck/actions/workflows/main.yml/badge.svg?branch=master"></a>
   <a href="https://coveralls.io/github/romainsacchi/carculator_truck" target="_blank"><img src="https://coveralls.io/repos/github/romainsacchi/carculator_truck/badge.svg"></a>
@@ -51,33 +51,37 @@
 <a href="https://www.simapro.com/" target="_blank">SimaPro 9.x.</a>.</li>
 </ul>
 
 <p align="center">
     The energy model of <i>carculator_truck</i> considers the vehicle aerodynamics, the road gradient and other factors.
     It also considers varying efficiencies of the transmission and engine at various load points for each second
     of the driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/energy_model.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/energy_model.png">
 </p>
 
 <p align="center">
     The energy model and the calculated tank-to-wheel energy consumption is validated against the simulation software
     <a href="https://ec.europa.eu/clima/policies/transport/vehicles/vecto_en" target="_blank">VECTO</a>.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/vecto_validation.png">
 </p>
 
 <p align="center">
     Benefits of hybrid powertrains are fully conidered: the possibility to recuperate braking energy as well as efficiency gains from engine
     downsizing is accounted for.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/hybrid_efficiency.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/hybrid_efficiency.png">
 </p>
 
 <p align="center">
     Global warming potential impacts per ton-km for a 40-t truck, across different powertrain technologies,
     using an urban driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png">
 </p>
 
 ## How to use it?
 
 See the notebook with [examples](https://github.com/romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb).
 
 ## Support
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 # ``carculator_truck``
-   [https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png]
+[https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                               mediumsmall.png]
      [https://badge.fury.io/py/carculator-truck.svg] [https://github.com/
            romainsacchi/carculator_truck/actions/workflows/main.yml/
    badge.svg?branch=master] [https://coveralls.io/repos/github/romainsacchi/
 carculator_truck/badge.svg] [https://readthedocs.org/projects/carculator_truck/
                             badge/?version=latest]
 Prospective environmental and economic life cycle assessment of medium and
 heavy duty vehicles. A fully parameterized Python model developed by the
@@ -32,26 +33,27 @@
       level but also in the rest of the world energy system (e.g., power
       generation) is accounted for, using energy scenario-specific IAM-coupled
       ecoinvent databases produced by premise.
     * Inventories can be imported into Brightway2 and SimaPro_9.x..
  The energy model of carculator_truck considers the vehicle aerodynamics, the
 road gradient and other factors. It also considers varying efficiencies of the
  transmission and engine at various load points for each second of the driving
-   cycle. [https://github.com/romainsacchi/carculator_truck/raw/master/docs/
-                               energy_model.png]
+  cycle. [https://github.com/romainsacchi/carculator_truck/blob/master/docs/
+                         _static/img/energy_model.png]
     The energy model and the calculated tank-to-wheel energy consumption is
      validated against the simulation software VECTO. [https://github.com/
-      romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png]
+          romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                             vecto_validation.png]
     Benefits of hybrid powertrains are fully conidered: the possibility to
 recuperate braking energy as well as efficiency gains from engine downsizing is
- accounted for. [https://github.com/romainsacchi/carculator_truck/raw/master/
-                          docs/hybrid_efficiency.png]
+ accounted for. [https://github.com/romainsacchi/carculator_truck/blob/master/
+                    docs/_static/img/hybrid_efficiency.png]
 Global warming potential impacts per ton-km for a 40-t truck, across different
   powertrain technologies, using an urban driving cycle. [https://github.com/
-         romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png]
+   romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png]
 ## How to use it? See the notebook with [examples](https://github.com/
 romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb). ## Support
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:
 carculator@psi.ch). ## Maintainers * [Romain Sacchi](https://github.com/
 romainsacchi) * [Chris Mutel](https://github.com/cmutel/) ## Contributing See
 [contributing](https://github.com/romainsacchi/carculator_truck/blob/master/
 CONTRIBUTING.md). ## License [BSD-3-Clause](https://github.com/romainsacchi/
```

### Comparing `carculator_truck-0.3.8/carculator_truck/background_systems.py` & `carculator_truck-0.3.9/carculator_truck/background_systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,22 +74,22 @@
         for s in scenario:
             val = df.loc[(df["Region"] == r) & (df["Scenario"] == s), "Biomass fuel":]
             array.loc[dict(region=r, scenario=s, value=0)] = val
     return array
 
 
 def get_electricity_mix():
-    """
-    Retrieve electricity mixes and shape them into an xarray.
+    """Retrieve electricity mixes and shape them into a xarray.
     Source:
-        * for European countries (`EU Reference Scenario 2016
-        <https://ec.europa.eu/energy/en/data-analysis/energy-modelling/eu-reference-scenario-2016>`_),
-        * for African countries (`TEMBA <http://www.osemosys.org/temba.html>`_ model)
-        * and for other countries (`IEA World Energy outlook 2017
-        <https://www.iea.org/reports/world-energy-outlook-2017>`_)
+
+    * for European countries (`EU Reference Scenario 2016
+      <https://op.europa.eu/en/publication-detail/-/publication/aed45f8e-63e3-47fb-9440-a0a14370f243/language-en/format-PDF/source-106883045>`_),
+    * for African countries (`TEMBA <http://www.osemosys.org/temba.html>`_ model)
+    * and for other countries (`IEA World Energy outlook 2017
+      <https://www.iea.org/reports/world-energy-outlook-2017>`_)
 
     :returns: An axarray with 'country' and 'year' as dimensions
     :rtype: xarray.core.dataarray.DataArray
 
     """
     filename = "electricity_mixes.csv"
     filepath = DATA_DIR / filename
@@ -200,17 +200,18 @@
 
 
 class BackgroundSystemModel:
     """
     Retrieve and build dictionaries that contain important information to model
     in the background system:
 
-        * gross electricity production mixes from nearly all countries in the world, from 2015 to 2050.
-        * cumulative electricity transformation/transmission/distribution losses from high voltage to medium and low voltage.
-        * share of biomass-derived fuel in the total consumption of liquid fuel in the transport sector. Source: REMIND.
+    * gross electricity production mixes from nearly all countries in the world, from 2015 to 2050.
+    * cumulative electricity transformation/transmission/distribution losses from high voltage to medium and low voltage.
+    * share of biomass-derived fuel in the total consumption of liquid fuel in the transport sector. Source: REMIND.
+
     """
 
     def __init__(self):
         self.electricity_mix = get_electricity_mix()
         self.losses = get_electricity_losses()
         self.region_map = get_region_mapping()
         self.biofuel = get_biofuel_share()
```

### Comparing `carculator_truck-0.3.8/carculator_truck/data/default_parameters.json` & `carculator_truck-0.3.9/carculator_truck/data/default_parameters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8365774265528476%*

 * *Differences: {"'1004-2000-power to mass ratio'": "{'minimum': 59.4, 'maximum': 72.60000000000001}",*

 * * "'1005-2010-power to mass ratio'": "{'minimum': 59.4, 'maximum': 72.60000000000001}",*

 * * "'1006-2020-power to mass ratio'": "{'minimum': 59.4, 'maximum': 72.60000000000001}",*

 * * "'1007-2030-power to mass ratio'": "{'minimum': 58.211999999999996, 'maximum': 71.148}",*

 * * "'1008-2040-power to mass ratio'": "{'minimum': 57.04776, 'maximum': 69.72503999999999}",*

 * * "'1009-2050-power to mass ratio'": "{'minimum': 55.906804799999996, ' […]*

```diff
@@ -264,16 +264,16 @@
     "1004-2000-power to mass ratio": {
         "amount": 66,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 66,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 72.60000000000001,
+        "minimum": 59.4,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -289,16 +289,16 @@
     "1005-2010-power to mass ratio": {
         "amount": 66,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 66,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 72.60000000000001,
+        "minimum": 59.4,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -314,16 +314,16 @@
     "1006-2020-power to mass ratio": {
         "amount": 66,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 66,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 72.60000000000001,
+        "minimum": 59.4,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -339,16 +339,16 @@
     "1007-2030-power to mass ratio": {
         "amount": 64.67999999999999,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 64.67999999999999,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 71.148,
+        "minimum": 58.211999999999996,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -364,16 +364,16 @@
     "1008-2040-power to mass ratio": {
         "amount": 63.386399999999995,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 63.386399999999995,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 69.72503999999999,
+        "minimum": 57.04776,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -389,16 +389,16 @@
     "1009-2050-power to mass ratio": {
         "amount": 62.118672,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 62.118672,
-        "maximum": 70,
-        "minimum": 50,
+        "maximum": 68.3305392,
+        "minimum": 55.906804799999996,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -449,16 +449,16 @@
     "1010-2000-power to mass ratio": {
         "amount": 38,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 38,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 41.800000000000004,
+        "minimum": 34.2,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -474,16 +474,16 @@
     "1011-2010-power to mass ratio": {
         "amount": 38,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 38,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 41.800000000000004,
+        "minimum": 34.2,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -499,16 +499,16 @@
     "1012-2020-power to mass ratio": {
         "amount": 38,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 38,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 41.800000000000004,
+        "minimum": 34.2,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -524,16 +524,16 @@
     "1013-2030-power to mass ratio": {
         "amount": 37.24,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 37.24,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 40.964000000000006,
+        "minimum": 33.516000000000005,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -549,16 +549,16 @@
     "1014-2040-power to mass ratio": {
         "amount": 36.495200000000004,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 36.495200000000004,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 40.14472000000001,
+        "minimum": 32.84568,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -574,16 +574,16 @@
     "1015-2050-power to mass ratio": {
         "amount": 35.765296000000006,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 35.765296000000006,
-        "maximum": 43,
-        "minimum": 30,
+        "maximum": 39.34182560000001,
+        "minimum": 32.188766400000006,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -599,16 +599,16 @@
     "1016-2000-power to mass ratio": {
         "amount": 35,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 35,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 38.5,
+        "minimum": 31.5,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -624,16 +624,16 @@
     "1017-2010-power to mass ratio": {
         "amount": 35,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 35,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 38.5,
+        "minimum": 31.5,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -649,16 +649,16 @@
     "1018-2020-power to mass ratio": {
         "amount": 35,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 35,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 38.5,
+        "minimum": 31.5,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -674,16 +674,16 @@
     "1019-2030-power to mass ratio": {
         "amount": 34.3,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 34.3,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 37.73,
+        "minimum": 30.869999999999997,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -699,16 +699,16 @@
     "102-2000-auxilliary power base demand": {
         "amount": 2205,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2205,
-        "maximum": 1212.75,
-        "minimum": 992.25,
+        "maximum": 2646,
+        "minimum": 1764,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -728,16 +728,16 @@
     "1020-2040-power to mass ratio": {
         "amount": 33.614,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 33.614,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 36.9754,
+        "minimum": 30.252599999999997,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -753,16 +753,16 @@
     "1021-2050-power to mass ratio": {
         "amount": 32.94172,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 32.94172,
-        "maximum": 44,
-        "minimum": 27,
+        "maximum": 36.235892,
+        "minimum": 29.647547999999997,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -778,16 +778,16 @@
     "1022-2000-power to mass ratio": {
         "amount": 29,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 29,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 31.900000000000002,
+        "minimum": 26.1,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -803,16 +803,16 @@
     "1023-2010-power to mass ratio": {
         "amount": 29,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 29,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 31.900000000000002,
+        "minimum": 26.1,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -828,16 +828,16 @@
     "1024-2020-power to mass ratio": {
         "amount": 29,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 29,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 31.900000000000002,
+        "minimum": 26.1,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -853,16 +853,16 @@
     "1025-2030-power to mass ratio": {
         "amount": 28.419999999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 28.419999999999998,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 31.262,
+        "minimum": 25.578,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -878,16 +878,16 @@
     "1026-2040-power to mass ratio": {
         "amount": 27.851599999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 27.851599999999998,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 30.63676,
+        "minimum": 25.06644,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -903,16 +903,16 @@
     "1027-2050-power to mass ratio": {
         "amount": 27.294567999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 27.294567999999998,
-        "maximum": 39,
-        "minimum": 26,
+        "maximum": 30.0240248,
+        "minimum": 24.5651112,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -928,16 +928,16 @@
     "1028-2000-power to mass ratio": {
         "amount": 28.5,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 28.5,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 31.35,
+        "minimum": 25.650000000000002,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -953,16 +953,16 @@
     "1029-2010-power to mass ratio": {
         "amount": 28.5,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 28.5,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 31.35,
+        "minimum": 25.650000000000002,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -978,16 +978,16 @@
     "103-2010-auxilliary power base demand": {
         "amount": 2100,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2100,
-        "maximum": 1155,
-        "minimum": 945,
+        "maximum": 2520,
+        "minimum": 1680,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -1007,16 +1007,16 @@
     "1030-2020-power to mass ratio": {
         "amount": 25,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 25,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 27.500000000000004,
+        "minimum": 22.5,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1032,16 +1032,16 @@
     "1031-2030-power to mass ratio": {
         "amount": 24.5,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.5,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 26.950000000000003,
+        "minimum": 22.05,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1057,16 +1057,16 @@
     "1032-2040-power to mass ratio": {
         "amount": 24.009999999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.009999999999998,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 26.411,
+        "minimum": 21.608999999999998,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1082,16 +1082,16 @@
     "1033-2050-power to mass ratio": {
         "amount": 23.529799999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 23.529799999999998,
-        "maximum": 30,
-        "minimum": 25,
+        "maximum": 25.88278,
+        "minimum": 21.17682,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1107,16 +1107,16 @@
     "1034-2000-power to mass ratio": {
         "amount": 28,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 28,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 30.800000000000004,
+        "minimum": 25.2,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1132,16 +1132,16 @@
     "1035-2010-power to mass ratio": {
         "amount": 28,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 28,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 30.800000000000004,
+        "minimum": 25.2,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1157,16 +1157,16 @@
     "1036-2020-power to mass ratio": {
         "amount": 25,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 25,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 27.500000000000004,
+        "minimum": 22.5,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1182,16 +1182,16 @@
     "1037-2030-power to mass ratio": {
         "amount": 24.5,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.5,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 26.950000000000003,
+        "minimum": 22.05,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1207,16 +1207,16 @@
     "1038-2040-power to mass ratio": {
         "amount": 24.009999999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.009999999999998,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 26.411,
+        "minimum": 21.608999999999998,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1232,16 +1232,16 @@
     "1039-2050-power to mass ratio": {
         "amount": 23.529799999999998,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 23.529799999999998,
-        "maximum": 33,
-        "minimum": 25,
+        "maximum": 25.88278,
+        "minimum": 21.17682,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1257,16 +1257,16 @@
     "104-2020-auxilliary power base demand": {
         "amount": 2000,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2000,
-        "maximum": 1100,
-        "minimum": 900,
+        "maximum": 2400,
+        "minimum": 1600,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -1286,16 +1286,16 @@
     "1040-2000-power to mass ratio": {
         "amount": 22,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 22,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 24.200000000000003,
+        "minimum": 19.8,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1311,16 +1311,16 @@
     "1041-2010-power to mass ratio": {
         "amount": 22,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 22,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 24.200000000000003,
+        "minimum": 19.8,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1336,16 +1336,16 @@
     "1042-2020-power to mass ratio": {
         "amount": 22,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 22,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 24.200000000000003,
+        "minimum": 19.8,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1361,16 +1361,16 @@
     "1043-2030-power to mass ratio": {
         "amount": 21.56,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 21.56,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 23.716,
+        "minimum": 19.404,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1386,16 +1386,16 @@
     "1044-2040-power to mass ratio": {
         "amount": 21.1288,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 21.1288,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 23.24168,
+        "minimum": 19.015919999999998,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1411,16 +1411,16 @@
     "1045-2050-power to mass ratio": {
         "amount": 20.706224,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 20.706224,
-        "maximum": 24,
-        "minimum": 20,
+        "maximum": 22.7768464,
+        "minimum": 18.6356016,
         "name": "power to mass ratio",
         "powertrain": [
             "ICEV-d",
             "ICEV-g",
             "HEV-d",
             "PHEV-c-d"
         ],
@@ -1528,16 +1528,16 @@
     "105-2030-auxilliary power base demand": {
         "amount": 1900,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 1900,
-        "maximum": 1045,
-        "minimum": 855,
+        "maximum": 2280,
+        "minimum": 1520,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -1557,15 +1557,15 @@
     "1050-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 70,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -1695,15 +1695,15 @@
     "1056-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 43,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -1787,16 +1787,16 @@
     "106-2040-auxilliary power base demand": {
         "amount": 1805,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 1805,
-        "maximum": 992.75,
-        "minimum": 812.25,
+        "maximum": 2166,
+        "minimum": 1444,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -1862,15 +1862,15 @@
     "1062-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 44,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -2000,15 +2000,15 @@
     "1068-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 39,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -2046,16 +2046,16 @@
     "107-2050-auxilliary power base demand": {
         "amount": 1714.75,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 1714.75,
-        "maximum": 943.1125,
-        "minimum": 771.6374999999999,
+        "maximum": 2057.7,
+        "minimum": 1371.8,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -2167,15 +2167,15 @@
     "1074-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 30,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -2305,16 +2305,16 @@
     "108-2000-auxilliary power base demand": {
         "amount": 3307.5,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3307.5,
-        "maximum": 2425.5,
-        "minimum": 1984.5,
+        "maximum": 3969,
+        "minimum": 2646,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -2334,15 +2334,15 @@
     "1080-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 33,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -2472,15 +2472,15 @@
     "1086-2040-power to mass ratio": {
         "amount": 24.9704,
         "category": "Glider",
         "comment": "calculated as power / curb mass",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 24.9704,
-        "maximum": 24,
+        "maximum": 27.467440000000003,
         "minimum": 22.473360000000003,
         "name": "power to mass ratio",
         "powertrain": [
             "BEV",
             "PHEV-e"
         ],
         "sizes": [
@@ -2562,16 +2562,16 @@
     "109-2010-auxilliary power base demand": {
         "amount": 3150,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3150,
-        "maximum": 2310,
-        "minimum": 1890,
+        "maximum": 3780,
+        "minimum": 2520,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -2840,16 +2840,16 @@
     "110-2020-auxilliary power base demand": {
         "amount": 3000,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3000,
-        "maximum": 2200,
-        "minimum": 1800,
+        "maximum": 3600,
+        "minimum": 2400,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -3089,16 +3089,16 @@
     "111-2030-auxilliary power base demand": {
         "amount": 2850,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2850,
-        "maximum": 2090,
-        "minimum": 1710,
+        "maximum": 3420,
+        "minimum": 2280,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -3338,16 +3338,16 @@
     "112-2040-auxilliary power base demand": {
         "amount": 2707.5,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2707.5,
-        "maximum": 1985.5,
-        "minimum": 1624.5,
+        "maximum": 3249,
+        "minimum": 2166,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -3587,16 +3587,16 @@
     "113-2050-auxilliary power base demand": {
         "amount": 2572.125,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 2572.125,
-        "maximum": 1886.225,
-        "minimum": 1543.2749999999999,
+        "maximum": 3086.5499999999997,
+        "minimum": 2057.7,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -3906,16 +3906,16 @@
     "114-2000-auxilliary power base demand": {
         "amount": 4410,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4410,
-        "maximum": 4630.5,
-        "minimum": 4189.5,
+        "maximum": 5292,
+        "minimum": 3528,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -4225,16 +4225,16 @@
     "115-2010-auxilliary power base demand": {
         "amount": 4200,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4200,
-        "maximum": 4410,
-        "minimum": 3990,
+        "maximum": 5040,
+        "minimum": 3360,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -4544,16 +4544,16 @@
     "116-2020-auxilliary power base demand": {
         "amount": 4000,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4000,
-        "maximum": 4200,
-        "minimum": 3800,
+        "maximum": 4800,
+        "minimum": 3200,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -4863,16 +4863,16 @@
     "117-2030-auxilliary power base demand": {
         "amount": 3800,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3800,
-        "maximum": 3990,
-        "minimum": 3610,
+        "maximum": 4560,
+        "minimum": 3040,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -5182,16 +5182,16 @@
     "118-2040-auxilliary power base demand": {
         "amount": 3610,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3610,
-        "maximum": 3790.5,
-        "minimum": 3429.5,
+        "maximum": 4332,
+        "minimum": 2888,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -5501,16 +5501,16 @@
     "119-2050-auxilliary power base demand": {
         "amount": 3429.5,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3429.5,
-        "maximum": 3600.975,
-        "minimum": 3258.0249999999996,
+        "maximum": 4115.4,
+        "minimum": 2743.6,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -5849,16 +5849,16 @@
     "120-2000-auxilliary power base demand": {
         "amount": 4630.5,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4630.5,
-        "maximum": 4851,
-        "minimum": 4410,
+        "maximum": 5556.6,
+        "minimum": 3704.4,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -6168,16 +6168,16 @@
     "121-2010-auxilliary power base demand": {
         "amount": 4410,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4410,
-        "maximum": 4620,
-        "minimum": 4200,
+        "maximum": 5292,
+        "minimum": 3528,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -6505,16 +6505,16 @@
     "122-2020-auxilliary power base demand": {
         "amount": 4200,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4200,
-        "maximum": 4400,
-        "minimum": 4000,
+        "maximum": 5040,
+        "minimum": 3360,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -6828,16 +6828,16 @@
     "123-2030-auxilliary power base demand": {
         "amount": 3990,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3990,
-        "maximum": 4180,
-        "minimum": 3800,
+        "maximum": 4788,
+        "minimum": 3192,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -7127,16 +7127,16 @@
     "124-2040-auxilliary power base demand": {
         "amount": 3790.5,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3790.5,
-        "maximum": 3971,
-        "minimum": 3610,
+        "maximum": 4548.599999999999,
+        "minimum": 3032.3999999999996,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -7426,16 +7426,16 @@
     "125-2050-auxilliary power base demand": {
         "amount": 3600.975,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3600.975,
-        "maximum": 3772.45,
-        "minimum": 3429.5,
+        "maximum": 4321.169999999999,
+        "minimum": 2880.7799999999997,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -7725,16 +7725,16 @@
     "126-2000-auxilliary power base demand": {
         "amount": 4961.25,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4961.25,
-        "maximum": 5292,
-        "minimum": 4630.5,
+        "maximum": 5953.5,
+        "minimum": 3969,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -8028,16 +8028,16 @@
     "127-2010-auxilliary power base demand": {
         "amount": 4725,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4725,
-        "maximum": 5040,
-        "minimum": 4410,
+        "maximum": 5670,
+        "minimum": 3780,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -8347,16 +8347,16 @@
     "128-2020-auxilliary power base demand": {
         "amount": 4500,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4500,
-        "maximum": 4800,
-        "minimum": 4200,
+        "maximum": 5400,
+        "minimum": 3600,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -8666,16 +8666,16 @@
     "129-2030-auxilliary power base demand": {
         "amount": 4275,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4275,
-        "maximum": 4560,
-        "minimum": 3990,
+        "maximum": 5130,
+        "minimum": 3420,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -9014,16 +9014,16 @@
     "130-2040-auxilliary power base demand": {
         "amount": 4061.25,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 4061.25,
-        "maximum": 4332,
-        "minimum": 3790.5,
+        "maximum": 4873.5,
+        "minimum": 3249,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -9333,16 +9333,16 @@
     "131-2050-auxilliary power base demand": {
         "amount": 3858.1875,
         "category": "Auxiliaries",
         "comment": "",
         "importance": "Limited",
         "kind": "distribution",
         "loc": 3858.1875,
-        "maximum": 4115.4,
-        "minimum": 3600.975,
+        "maximum": 4629.825,
+        "minimum": 3086.5499999999997,
         "name": "auxilliary power base demand",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -17628,17 +17628,23 @@
         "maximum": 0.45,
         "minimum": 0.35,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
-            "3.5t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
     "1569-2010-fuel cell stack efficiency": {
         "amount": 0.5,
@@ -17650,17 +17656,23 @@
         "maximum": 0.55,
         "minimum": 0.45,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
-            "3.5t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
     "157-2010-toll cost per km": {
         "amount": 0.018,
@@ -17688,293 +17700,126 @@
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
         "year": 2010
     },
     "1570-2020-fuel cell stack efficiency": {
-        "amount": 0.6,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.6,
-        "maximum": 0.66,
-        "minimum": 0.54,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1571-2030-fuel cell stack efficiency": {
-        "amount": 0.6,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.6,
-        "maximum": 0.66,
-        "minimum": 0.54,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1572-2040-fuel cell stack efficiency": {
-        "amount": 0.6,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.6,
-        "maximum": 0.66,
-        "minimum": 0.54,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1573-2050-fuel cell stack efficiency": {
-        "amount": 0.6,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.6,
-        "maximum": 0.66,
-        "minimum": 0.54,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1574-2000-fuel cell stack efficiency": {
-        "amount": 0.35000000000000003,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.35000000000000003,
-        "maximum": 0.4,
-        "minimum": 0.3,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t",
-            "18t",
-            "26t",
-            "32t",
-            "40t",
-            "60t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1575-2010-fuel cell stack efficiency": {
-        "amount": 0.45,
-        "category": "Powertrain",
-        "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.45,
-        "maximum": 0.5,
-        "minimum": 0.4,
-        "name": "fuel cell stack efficiency",
-        "powertrain": [
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t",
-            "18t",
-            "26t",
-            "32t",
-            "40t",
-            "60t"
-        ],
-        "source": "Cox et al. 2020",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "1576-2020-fuel cell stack efficiency": {
-        "amount": 0.54,
+        "amount": 0.55,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.54,
-        "maximum": 0.5940000000000001,
-        "minimum": 0.48600000000000004,
+        "loc": 0.55,
+        "maximum": 0.6,
+        "minimum": 0.5,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
+            "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
             "40t",
             "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1577-2030-fuel cell stack efficiency": {
-        "amount": 0.55,
+    "1571-2030-fuel cell stack efficiency": {
+        "amount": 0.6,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.55,
-        "maximum": 0.6050000000000001,
-        "minimum": 0.49500000000000005,
+        "loc": 0.6,
+        "maximum": 0.65,
+        "minimum": 0.55,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
+            "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
             "40t",
             "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1578-2040-fuel cell stack efficiency": {
-        "amount": 0.56,
+    "1572-2040-fuel cell stack efficiency": {
+        "amount": 0.65,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.56,
-        "maximum": 0.6160000000000001,
-        "minimum": 0.5040000000000001,
+        "loc": 0.65,
+        "maximum": 0.7,
+        "minimum": 0.6,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
+            "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
             "40t",
             "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1579-2050-fuel cell stack efficiency": {
-        "amount": 0.57,
+    "1573-2050-fuel cell stack efficiency": {
+        "amount": 0.7,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040.",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.57,
-        "maximum": 0.627,
-        "minimum": 0.513,
+        "loc": 0.7,
+        "maximum": 0.75,
+        "minimum": 0.65,
         "name": "fuel cell stack efficiency",
         "powertrain": [
             "FCEV"
         ],
         "sizes": [
+            "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
             "40t",
             "60t"
         ],
-        "source": "Cox et al. 2020",
+        "source": "Cox et al. 2020, https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "158-2020-toll cost per km": {
-        "amount": 0.018,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.018,
-        "maximum": 0.021599999999999998,
-        "minimum": 0.0144,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2020
-    },
-    "1580-2000-fuel cell power share": {
+    "1574-2000-fuel cell power share": {
         "amount": 0.25,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.25,
         "maximum": 0.3,
@@ -17992,15 +17837,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1581-2010-fuel cell power share": {
+    "1575-2010-fuel cell power share": {
         "amount": 0.25,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.25,
         "maximum": 0.3,
@@ -18018,15 +17863,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1582-2020-fuel cell power share": {
+    "1576-2020-fuel cell power share": {
         "amount": 0.25,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.25,
         "maximum": 0.3,
@@ -18044,15 +17889,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1583-2030-fuel cell power share": {
+    "1577-2030-fuel cell power share": {
         "amount": 0.35,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.35,
         "maximum": 0.4,
@@ -18070,15 +17915,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1584-2040-fuel cell power share": {
+    "1578-2040-fuel cell power share": {
         "amount": 0.35,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.35,
         "maximum": 0.4,
@@ -18096,15 +17941,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1585-2050-fuel cell power share": {
+    "1579-2050-fuel cell power share": {
         "amount": 0.25,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.25,
         "maximum": 0.3,
@@ -18122,15 +17967,44 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1586-2000-fuel cell power share": {
+    "158-2020-toll cost per km": {
+        "amount": 0.018,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.018,
+        "maximum": 0.021599999999999998,
+        "minimum": 0.0144,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2020
+    },
+    "1580-2000-fuel cell power share": {
         "amount": 0.2,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.2,
         "maximum": 0.25,
@@ -18145,15 +18019,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1587-2010-fuel cell power share": {
+    "1581-2010-fuel cell power share": {
         "amount": 0.2,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.2,
         "maximum": 0.25,
@@ -18168,15 +18042,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1588-2020-fuel cell power share": {
+    "1582-2020-fuel cell power share": {
         "amount": 0.2,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.2,
         "maximum": 0.25,
@@ -18191,15 +18065,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1589-2030-fuel cell power share": {
+    "1583-2030-fuel cell power share": {
         "amount": 0.3,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.3,
         "maximum": 0.35000000000000003,
@@ -18214,44 +18088,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "159-2030-toll cost per km": {
-        "amount": 0.018,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.018,
-        "maximum": 0.021599999999999998,
-        "minimum": 0.0144,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2030
-    },
-    "1590-2040-fuel cell power share": {
+    "1584-2040-fuel cell power share": {
         "amount": 0.3,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.3,
         "maximum": 0.35000000000000003,
@@ -18266,15 +18111,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1591-2050-fuel cell power share": {
+    "1585-2050-fuel cell power share": {
         "amount": 0.2,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.2,
         "maximum": 0.25,
@@ -18289,15 +18134,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1592-2000-fuel cell power area density": {
+    "1586-2000-fuel cell power area density": {
         "amount": 350,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 350,
         "maximum": 450,
@@ -18317,15 +18162,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2000
     },
-    "1593-2010-fuel cell power area density": {
+    "1587-2010-fuel cell power area density": {
         "amount": 400,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 400,
         "maximum": 500,
@@ -18345,15 +18190,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2010
     },
-    "1594-2020-fuel cell power area density": {
+    "1588-2020-fuel cell power area density": {
         "amount": 450,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 450,
         "maximum": 550,
@@ -18373,15 +18218,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2020
     },
-    "1595-2030-fuel cell power area density": {
+    "1589-2030-fuel cell power area density": {
         "amount": 450,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 450,
         "maximum": 550,
@@ -18401,15 +18246,44 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2030
     },
-    "1596-2040-fuel cell power area density": {
+    "159-2030-toll cost per km": {
+        "amount": 0.018,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.018,
+        "maximum": 0.021599999999999998,
+        "minimum": 0.0144,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2030
+    },
+    "1590-2040-fuel cell power area density": {
         "amount": 500,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 500,
         "maximum": 600,
@@ -18429,15 +18303,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2040
     },
-    "1597-2050-fuel cell power area density": {
+    "1591-2050-fuel cell power area density": {
         "amount": 600,
         "category": "Powertrain",
         "comment": "own assumption for 2000, 2010, 2050. Cox et al. 2020 for 2020, 2040. Assumed to be half that of passenger cars.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 600,
         "maximum": 700,
@@ -18457,15 +18331,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "mW/cm2",
         "year": 2050
     },
-    "1598-2000-fuel cell own consumption": {
+    "1592-2000-fuel cell own consumption": {
         "amount": 1.2,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.2,
         "maximum": 1.25,
@@ -18485,15 +18359,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2000
     },
-    "1599-2010-fuel cell own consumption": {
+    "1593-2010-fuel cell own consumption": {
         "amount": 1.175,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.175,
         "maximum": 1.2,
@@ -18513,73 +18387,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2010
     },
-    "16-2040-heating thermal demand": {
-        "amount": 213.75,
-        "category": "Auxiliaries",
-        "comment": "own assumption",
-        "importance": "Limited",
-        "kind": "distribution",
-        "loc": 213.75,
-        "maximum": 270,
-        "minimum": 162,
-        "name": "heating thermal demand",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "W",
-        "year": 2040
-    },
-    "160-2040-toll cost per km": {
-        "amount": 0.018,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.018,
-        "maximum": 0.021599999999999998,
-        "minimum": 0.0144,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2040
-    },
-    "1600-2020-fuel cell own consumption": {
+    "1594-2020-fuel cell own consumption": {
         "amount": 1.15,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.15,
         "maximum": 1.175,
@@ -18599,15 +18415,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2020
     },
-    "1601-2030-fuel cell own consumption": {
+    "1595-2030-fuel cell own consumption": {
         "amount": 1.125,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.125,
         "maximum": 1.1475,
@@ -18627,15 +18443,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2030
     },
-    "1602-2040-fuel cell own consumption": {
+    "1596-2040-fuel cell own consumption": {
         "amount": 1.1,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.1,
         "maximum": 1.122,
@@ -18655,15 +18471,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2040
     },
-    "1603-2050-fuel cell own consumption": {
+    "1597-2050-fuel cell own consumption": {
         "amount": 1.075,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.075,
         "maximum": 1.0965,
@@ -18683,15 +18499,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kW/kW",
         "year": 2050
     },
-    "1604-2000-fuel cell essential BoP mass per power": {
+    "1598-2000-fuel cell essential BoP mass per power": {
         "amount": 1.1025,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.1025,
         "maximum": 1.4332500000000004,
@@ -18711,15 +18527,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2000
     },
-    "1605-2010-fuel cell essential BoP mass per power": {
+    "1599-2010-fuel cell essential BoP mass per power": {
         "amount": 1.05,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1.05,
         "maximum": 1.3650000000000002,
@@ -18739,15 +18555,73 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2010
     },
-    "1606-2020-fuel cell essential BoP mass per power": {
+    "16-2040-heating thermal demand": {
+        "amount": 213.75,
+        "category": "Auxiliaries",
+        "comment": "own assumption",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 213.75,
+        "maximum": 270,
+        "minimum": 162,
+        "name": "heating thermal demand",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "",
+        "status": "To be improved",
+        "uncertainty_type": 5,
+        "unit": "W",
+        "year": 2040
+    },
+    "160-2040-toll cost per km": {
+        "amount": 0.018,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.018,
+        "maximum": 0.021599999999999998,
+        "minimum": 0.0144,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2040
+    },
+    "1600-2020-fuel cell essential BoP mass per power": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 1,
         "maximum": 1.3,
@@ -18767,15 +18641,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2020
     },
-    "1607-2030-fuel cell essential BoP mass per power": {
+    "1601-2030-fuel cell essential BoP mass per power": {
         "amount": 0.85,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.85,
         "maximum": 0.95,
@@ -18795,15 +18669,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2030
     },
-    "1608-2040-fuel cell essential BoP mass per power": {
+    "1602-2040-fuel cell essential BoP mass per power": {
         "amount": 0.7,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.7,
         "maximum": 1,
@@ -18823,15 +18697,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2040
     },
-    "1609-2050-fuel cell essential BoP mass per power": {
+    "1603-2050-fuel cell essential BoP mass per power": {
         "amount": 0.6649999999999999,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.6649999999999999,
         "maximum": 0.95,
@@ -18851,44 +18725,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2050
     },
-    "161-2050-toll cost per km": {
-        "amount": 0.018,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.018,
-        "maximum": 0.021599999999999998,
-        "minimum": 0.0144,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2050
-    },
-    "1610-2000-fuel cell ancillary BoP mass per power": {
+    "1604-2000-fuel cell ancillary BoP mass per power": {
         "amount": 0.44100000000000006,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.44100000000000006,
         "maximum": 0.49612500000000004,
@@ -18908,15 +18753,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2000
     },
-    "1611-2010-fuel cell ancillary BoP mass per power": {
+    "1605-2010-fuel cell ancillary BoP mass per power": {
         "amount": 0.42000000000000004,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.42000000000000004,
         "maximum": 0.47250000000000003,
@@ -18936,15 +18781,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2010
     },
-    "1612-2020-fuel cell ancillary BoP mass per power": {
+    "1606-2020-fuel cell ancillary BoP mass per power": {
         "amount": 0.4,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.4,
         "maximum": 0.45,
@@ -18964,15 +18809,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2020
     },
-    "1613-2030-fuel cell ancillary BoP mass per power": {
+    "1607-2030-fuel cell ancillary BoP mass per power": {
         "amount": 0.35,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.35,
         "maximum": 0.4,
@@ -18992,15 +18837,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2030
     },
-    "1614-2040-fuel cell ancillary BoP mass per power": {
+    "1608-2040-fuel cell ancillary BoP mass per power": {
         "amount": 0.3,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.3,
         "maximum": 0.34,
@@ -19020,15 +18865,15 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2040
     },
-    "1615-2050-fuel cell ancillary BoP mass per power": {
+    "1609-2050-fuel cell ancillary BoP mass per power": {
         "amount": 0.285,
         "category": "Powertrain",
         "comment": "",
         "importance": "",
         "kind": "distribution",
         "loc": 0.285,
         "maximum": 0.323,
@@ -19048,15 +18893,44 @@
         ],
         "source": "",
         "status": "",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2050
     },
-    "1616-2000-engine mass per power": {
+    "161-2050-toll cost per km": {
+        "amount": 0.018,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.018,
+        "maximum": 0.021599999999999998,
+        "minimum": 0.0144,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2050
+    },
+    "1610-2000-engine mass per power": {
         "amount": 3.087,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 3.087,
         "maximum": 3.8587500000000006,
@@ -19078,15 +18952,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2000
     },
-    "1617-2010-engine mass per power": {
+    "1611-2010-engine mass per power": {
         "amount": 2.94,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.94,
         "maximum": 3.6750000000000003,
@@ -19108,15 +18982,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2010
     },
-    "1618-2020-engine mass per power": {
+    "1612-2020-engine mass per power": {
         "amount": 2.8,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.8,
         "maximum": 3.5,
@@ -19138,15 +19012,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2020
     },
-    "1619-2030-engine mass per power": {
+    "1613-2030-engine mass per power": {
         "amount": 2.8,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.8,
         "maximum": 3.3249999999999997,
@@ -19168,44 +19042,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2030
     },
-    "162-2000-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2000
-    },
-    "1620-2040-engine mass per power": {
+    "1614-2040-engine mass per power": {
         "amount": 2.8,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.8,
         "maximum": 3.1587499999999995,
@@ -19227,15 +19072,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2040
     },
-    "1621-2050-engine mass per power": {
+    "1615-2050-engine mass per power": {
         "amount": 2.8,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.8,
         "maximum": 3.0008124999999994,
@@ -19257,15 +19102,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2050
     },
-    "1622-2000-engine mass per power": {
+    "1616-2000-engine mass per power": {
         "amount": 3.19725,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 3.19725,
         "maximum": 3.8587500000000006,
@@ -19285,15 +19130,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2000
     },
-    "1623-2010-engine mass per power": {
+    "1617-2010-engine mass per power": {
         "amount": 3.045,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 3.045,
         "maximum": 3.6750000000000003,
@@ -19313,15 +19158,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2010
     },
-    "1624-2020-engine mass per power": {
+    "1618-2020-engine mass per power": {
         "amount": 2.9,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.9,
         "maximum": 3.5,
@@ -19341,15 +19186,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2020
     },
-    "1625-2030-engine mass per power": {
+    "1619-2030-engine mass per power": {
         "amount": 2.9,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.9,
         "maximum": 3.3249999999999997,
@@ -19369,15 +19214,44 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2030
     },
-    "1626-2040-engine mass per power": {
+    "162-2000-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2000
+    },
+    "1620-2040-engine mass per power": {
         "amount": 2.9,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.9,
         "maximum": 3.1587499999999995,
@@ -19397,15 +19271,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2040
     },
-    "1627-2050-engine mass per power": {
+    "1621-2050-engine mass per power": {
         "amount": 2.9,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 2.9,
         "maximum": 3.0008124999999994,
@@ -19425,15 +19299,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2050
     },
-    "1628-2000-engine fixed mass": {
+    "1622-2000-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19453,15 +19327,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2000
     },
-    "1629-2010-engine fixed mass": {
+    "1623-2010-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19481,44 +19355,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2010
     },
-    "163-2010-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2010
-    },
-    "1630-2020-engine fixed mass": {
+    "1624-2020-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19538,15 +19383,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2020
     },
-    "1631-2030-engine fixed mass": {
+    "1625-2030-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19566,15 +19411,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2030
     },
-    "1632-2040-engine fixed mass": {
+    "1626-2040-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19594,15 +19439,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2040
     },
-    "1633-2050-engine fixed mass": {
+    "1627-2050-engine fixed mass": {
         "amount": 50,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 50,
         "name": "engine fixed mass",
@@ -19622,15 +19467,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2050
     },
-    "1634-2000-engine fixed mass": {
+    "1628-2000-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19648,15 +19493,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2000
     },
-    "1635-2010-engine fixed mass": {
+    "1629-2010-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19674,15 +19519,44 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2010
     },
-    "1636-2020-engine fixed mass": {
+    "163-2010-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2010
+    },
+    "1630-2020-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19700,15 +19574,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2020
     },
-    "1637-2030-engine fixed mass": {
+    "1631-2030-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19726,15 +19600,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2030
     },
-    "1638-2040-engine fixed mass": {
+    "1632-2040-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19752,15 +19626,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2040
     },
-    "1639-2050-engine fixed mass": {
+    "1633-2050-engine fixed mass": {
         "amount": 157,
         "category": "Powertrain",
         "comment": "Based on seven heavy duty combustion engines (3 Cummins, 1 Isuzu, 3 Peterbilt), from 220 to 400kW",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 157,
         "name": "engine fixed mass",
@@ -19778,44 +19652,15 @@
         ],
         "source": "https://www.cervusequipment.com/peterbilt/new-trucks/engines/",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2050
     },
-    "164-2020-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2020
-    },
-    "1640-2000-CNG engine efficiency correction factor": {
+    "1634-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -19829,15 +19674,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1641-2010-CNG engine efficiency correction factor": {
+    "1635-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -19851,15 +19696,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1642-2020-CNG engine efficiency correction factor": {
+    "1636-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -19873,15 +19718,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1643-2030-CNG engine efficiency correction factor": {
+    "1637-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -19895,15 +19740,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1644-2040-CNG engine efficiency correction factor": {
+    "1638-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -19917,15 +19762,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1645-2050-CNG engine efficiency correction factor": {
+    "1639-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -19939,15 +19784,44 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1646-2000-CNG engine efficiency correction factor": {
+    "164-2020-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2020
+    },
+    "1640-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -19961,15 +19835,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1647-2010-CNG engine efficiency correction factor": {
+    "1641-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -19983,15 +19857,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1648-2020-CNG engine efficiency correction factor": {
+    "1642-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20005,15 +19879,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1649-2030-CNG engine efficiency correction factor": {
+    "1643-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20027,44 +19901,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "165-2030-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2030
-    },
-    "1650-2040-CNG engine efficiency correction factor": {
+    "1644-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20078,15 +19923,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1651-2050-CNG engine efficiency correction factor": {
+    "1645-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20100,15 +19945,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1652-2000-CNG engine efficiency correction factor": {
+    "1646-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20122,15 +19967,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1653-2010-CNG engine efficiency correction factor": {
+    "1647-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20144,15 +19989,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1654-2020-CNG engine efficiency correction factor": {
+    "1648-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20166,15 +20011,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1655-2030-CNG engine efficiency correction factor": {
+    "1649-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20188,15 +20033,44 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1656-2040-CNG engine efficiency correction factor": {
+    "165-2030-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2030
+    },
+    "1650-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20210,15 +20084,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1657-2050-CNG engine efficiency correction factor": {
+    "1651-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20232,15 +20106,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1658-2000-CNG engine efficiency correction factor": {
+    "1652-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20254,15 +20128,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1659-2010-CNG engine efficiency correction factor": {
+    "1653-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20276,44 +20150,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "166-2040-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2040
-    },
-    "1660-2020-CNG engine efficiency correction factor": {
+    "1654-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20327,15 +20172,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1661-2030-CNG engine efficiency correction factor": {
+    "1655-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20349,15 +20194,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1662-2040-CNG engine efficiency correction factor": {
+    "1656-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20371,15 +20216,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1663-2050-CNG engine efficiency correction factor": {
+    "1657-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20393,15 +20238,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1664-2000-CNG engine efficiency correction factor": {
+    "1658-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20415,15 +20260,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1665-2010-CNG engine efficiency correction factor": {
+    "1659-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20437,15 +20282,44 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1666-2020-CNG engine efficiency correction factor": {
+    "166-2040-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2040
+    },
+    "1660-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20459,15 +20333,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1667-2030-CNG engine efficiency correction factor": {
+    "1661-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20481,15 +20355,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1668-2040-CNG engine efficiency correction factor": {
+    "1662-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20503,15 +20377,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1669-2050-CNG engine efficiency correction factor": {
+    "1663-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20525,44 +20399,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "167-2050-toll cost per km": {
-        "amount": 0.051,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.051,
-        "maximum": 0.06119999999999999,
-        "minimum": 0.0408,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2050
-    },
-    "1670-2000-CNG engine efficiency correction factor": {
+    "1664-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20576,15 +20421,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1671-2010-CNG engine efficiency correction factor": {
+    "1665-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20598,15 +20443,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1672-2020-CNG engine efficiency correction factor": {
+    "1666-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20620,15 +20465,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1673-2030-CNG engine efficiency correction factor": {
+    "1667-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20642,15 +20487,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1674-2040-CNG engine efficiency correction factor": {
+    "1668-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20664,15 +20509,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1675-2050-CNG engine efficiency correction factor": {
+    "1669-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20686,15 +20531,44 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1676-2000-CNG engine efficiency correction factor": {
+    "167-2050-toll cost per km": {
+        "amount": 0.051,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.051,
+        "maximum": 0.06119999999999999,
+        "minimum": 0.0408,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2050
+    },
+    "1670-2000-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20708,15 +20582,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1677-2010-CNG engine efficiency correction factor": {
+    "1671-2010-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20730,15 +20604,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1678-2020-CNG engine efficiency correction factor": {
+    "1672-2020-CNG engine efficiency correction factor": {
         "amount": 0.1,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.1,
         "maximum": 0.13,
@@ -20752,15 +20626,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1679-2030-CNG engine efficiency correction factor": {
+    "1673-2030-CNG engine efficiency correction factor": {
         "amount": 0.05,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.05,
         "maximum": 0.06,
@@ -20774,44 +20648,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "168-2000-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2000
-    },
-    "1680-2040-CNG engine efficiency correction factor": {
+    "1674-2040-CNG engine efficiency correction factor": {
         "amount": 0.025,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.025,
         "maximum": 0.03,
@@ -20825,15 +20670,15 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1681-2050-CNG engine efficiency correction factor": {
+    "1675-2050-CNG engine efficiency correction factor": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Based on ICCT analysis on EU trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "maximum": 0.05,
@@ -20847,505 +20692,155 @@
         ],
         "source": "Correction factor for CNG from https://theicct.org/sites/default/files/publications/eu-hdv-co2-standards-baseline-data-sept21.pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1682-2000-engine efficiency": {
+    "1676-2000-engine efficiency": {
         "amount": 0.93,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.93,
         "maximum": 0.95,
         "minimum": 0.8370000000000001,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1683-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "1684-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1685-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1686-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1687-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "3.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1688-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
+            "ICEV-d",
+            "ICEV-g",
             "BEV",
-            "PHEV-e",
-            "FCEV"
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
-            "7.5t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1689-2010-engine efficiency": {
+    "1677-2010-engine efficiency": {
         "amount": 0.93,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.93,
         "maximum": 0.95,
         "minimum": 0.8370000000000001,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "169-2010-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "32t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2010
-    },
-    "1690-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1691-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1692-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1693-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "7.5t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1694-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1695-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "18t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1696-2020-engine efficiency": {
+    "1678-2020-engine efficiency": {
         "amount": 0.93,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.93,
         "maximum": 0.95,
         "minimum": 0.8370000000000001,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
-            "18t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1697-2030-engine efficiency": {
+    "1679-2030-engine efficiency": {
         "amount": 0.935,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.935,
         "maximum": 0.95,
         "minimum": 0.8415,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1698-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1699-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "18t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "17-2050-heating thermal demand": {
-        "amount": 213.75,
-        "category": "Auxiliaries",
-        "comment": "own assumption",
-        "importance": "Limited",
-        "kind": "distribution",
-        "loc": 213.75,
-        "maximum": 270,
-        "minimum": 162,
-        "name": "heating thermal demand",
-        "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "18t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
-        "source": "",
+        "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
-        "unit": "W",
-        "year": 2050
+        "unit": "unitless",
+        "year": 2030
     },
-    "170-2020-toll cost per km": {
+    "168-2000-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
         "maximum": 0.0384,
@@ -21364,664 +20859,105 @@
         "sizes": [
             "32t"
         ],
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
-        "year": 2020
-    },
-    "1700-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
         "year": 2000
     },
-    "1701-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "1702-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1703-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1704-2040-engine efficiency": {
+    "1680-2040-engine efficiency": {
         "amount": 0.94,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.94,
         "maximum": 0.96,
         "minimum": 0.846,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1705-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1706-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1707-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "1708-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1709-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "171-2030-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "32t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2030
-    },
-    "1710-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1711-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1712-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1713-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "1714-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1715-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1716-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1717-2050-engine efficiency": {
+    "1681-2050-engine efficiency": {
         "amount": 0.945,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.945,
         "maximum": 0.96,
         "minimum": 0.8504999999999999,
         "name": "engine efficiency",
         "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2050
-    },
-    "1718-2000-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2000
-    },
-    "1719-2010-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2010
-    },
-    "172-2040-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "32t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2040
-    },
-    "1720-2020-engine efficiency": {
-        "amount": 0.93,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.93,
-        "maximum": 0.95,
-        "minimum": 0.8370000000000001,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1721-2030-engine efficiency": {
-        "amount": 0.935,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.935,
-        "maximum": 0.95,
-        "minimum": 0.8415,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
-    },
-    "1722-2040-engine efficiency": {
-        "amount": 0.94,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.94,
-        "maximum": 0.96,
-        "minimum": 0.846,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "https://doi.org/10.3141%2F2539-07",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2040
-    },
-    "1723-2050-engine efficiency": {
-        "amount": 0.945,
-        "category": "Powertrain",
-        "comment": "Based on electric buses",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.945,
-        "maximum": 0.96,
-        "minimum": 0.8504999999999999,
-        "name": "engine efficiency",
-        "powertrain": [
-            "BEV",
-            "PHEV-e",
-            "FCEV"
-        ],
-        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
             "60t"
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1724-2000-transmission efficiency": {
+    "1682-2000-transmission efficiency": {
         "amount": 0.89,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.89,
         "maximum": 0.95,
         "minimum": 0.801,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22030,28 +20966,33 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1725-2010-transmission efficiency": {
+    "1683-2010-transmission efficiency": {
         "amount": 0.89,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.89,
         "maximum": 0.95,
         "minimum": 0.801,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22060,28 +21001,33 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1726-2020-transmission efficiency": {
+    "1684-2020-transmission efficiency": {
         "amount": 0.89,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.89,
         "maximum": 0.9790000000000001,
         "minimum": 0.801,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22090,28 +21036,33 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1727-2030-transmission efficiency": {
+    "1685-2030-transmission efficiency": {
         "amount": 0.9,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.9,
         "maximum": 0.9900000000000001,
         "minimum": 0.81,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22120,28 +21071,33 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1728-2040-transmission efficiency": {
+    "1686-2040-transmission efficiency": {
         "amount": 0.91,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.91,
         "maximum": 0.96,
         "minimum": 0.8190000000000001,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22150,28 +21106,33 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1729-2050-transmission efficiency": {
+    "1687-2050-transmission efficiency": {
         "amount": 0.92,
         "category": "Powertrain",
         "comment": "Based on electric buses",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.92,
         "maximum": 0.97,
         "minimum": 0.8280000000000001,
         "name": "transmission efficiency",
         "powertrain": [
-            "BEV",
+            "PHEV-c-d",
             "PHEV-e",
-            "FCEV"
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -22180,44 +21141,15 @@
         ],
         "source": "https://doi.org/10.3141%2F2539-07",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "173-2050-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "32t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2050
-    },
-    "1730-2000-emotor mass per power": {
+    "1688-2000-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22244,15 +21176,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2000
     },
-    "1731-2010-emotor mass per power": {
+    "1689-2010-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22279,15 +21211,44 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2010
     },
-    "1732-2020-emotor mass per power": {
+    "169-2010-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "32t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2010
+    },
+    "1690-2020-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22314,15 +21275,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2020
     },
-    "1733-2030-emotor mass per power": {
+    "1691-2030-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22349,15 +21310,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2030
     },
-    "1734-2040-emotor mass per power": {
+    "1692-2040-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22384,15 +21345,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2040
     },
-    "1735-2050-emotor mass per power": {
+    "1693-2050-emotor mass per power": {
         "amount": 1.46,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 1.46,
         "maximum": 1.5,
@@ -22419,15 +21380,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg/kW",
         "year": 2050
     },
-    "1736-2000-emotor fixed mass": {
+    "1694-2000-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22452,15 +21413,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2000
     },
-    "1737-2010-emotor fixed mass": {
+    "1695-2010-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22485,15 +21446,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2010
     },
-    "1738-2020-emotor fixed mass": {
+    "1696-2020-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22518,15 +21479,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2020
     },
-    "1739-2030-emotor fixed mass": {
+    "1697-2030-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22551,44 +21512,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2030
     },
-    "174-2000-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2000
-    },
-    "1740-2040-emotor fixed mass": {
+    "1698-2040-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22613,15 +21545,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2040
     },
-    "1741-2050-emotor fixed mass": {
+    "1699-2050-emotor fixed mass": {
         "amount": -59,
         "category": "Powertrain",
         "comment": "Based on four Brusa motors: 28kW, 70kW, 93kW and 145kW\nAnd a 400kW motor from Wolff et al. 2020",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": -59,
         "name": "emotor fixed mass",
@@ -22646,15 +21578,73 @@
         ],
         "source": "https://www.brusa.biz/en/products/drive/motor-400-v/hsm1-101822.html",
         "status": "Acceptable",
         "uncertainty_type": 1,
         "unit": "kg",
         "year": 2050
     },
-    "1742-2000-converter mass": {
+    "17-2050-heating thermal demand": {
+        "amount": 213.75,
+        "category": "Auxiliaries",
+        "comment": "own assumption",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 213.75,
+        "maximum": 270,
+        "minimum": 162,
+        "name": "heating thermal demand",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "18t"
+        ],
+        "source": "",
+        "status": "To be improved",
+        "uncertainty_type": 5,
+        "unit": "W",
+        "year": 2050
+    },
+    "170-2020-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "32t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2020
+    },
+    "1700-2000-converter mass": {
         "amount": 35,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 35,
         "maximum": 40,
@@ -22676,15 +21666,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2000
     },
-    "1743-2010-converter mass": {
+    "1701-2010-converter mass": {
         "amount": 30,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 30,
         "maximum": 35,
@@ -22706,15 +21696,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2010
     },
-    "1744-2020-converter mass": {
+    "1702-2020-converter mass": {
         "amount": 25,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 25,
         "maximum": 30,
@@ -22736,15 +21726,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2020
     },
-    "1745-2030-converter mass": {
+    "1703-2030-converter mass": {
         "amount": 25,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 25,
         "maximum": 30,
@@ -22766,15 +21756,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2030
     },
-    "1746-2040-converter mass": {
+    "1704-2040-converter mass": {
         "amount": 23.75,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 23.75,
         "maximum": 30,
@@ -22796,15 +21786,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2040
     },
-    "1747-2050-converter mass": {
+    "1705-2050-converter mass": {
         "amount": 22.5625,
         "category": "Powertrain",
         "comment": "Fit BEV and FCEV buses.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 22.5625,
         "maximum": 28.5,
@@ -22826,15 +21816,15 @@
         ],
         "source": "https://www.brusa.biz/en/products/dcdc-converter/hvhv-800-v/bdc546.html",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2050
     },
-    "1748-2000-combustion power share": {
+    "1706-2000-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -22848,15 +21838,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1749-2010-combustion power share": {
+    "1707-2010-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -22870,15 +21860,59 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "175-2010-toll cost per km": {
+    "1708-2020-combustion power share": {
+        "amount": 0.67,
+        "category": "Powertrain",
+        "comment": "Based on US trucks",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 0.67,
+        "maximum": 0.75,
+        "minimum": 0.65,
+        "name": "combustion power share",
+        "powertrain": [
+            "HEV-d"
+        ],
+        "sizes": [
+            "3.5t"
+        ],
+        "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
+        "status": "To be improved",
+        "uncertainty_type": 5,
+        "unit": "unitless",
+        "year": 2020
+    },
+    "1709-2030-combustion power share": {
+        "amount": 0.67,
+        "category": "Powertrain",
+        "comment": "Based on US trucks",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 0.67,
+        "maximum": 0.75,
+        "minimum": 0.65,
+        "name": "combustion power share",
+        "powertrain": [
+            "HEV-d"
+        ],
+        "sizes": [
+            "3.5t"
+        ],
+        "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
+        "status": "To be improved",
+        "uncertainty_type": 5,
+        "unit": "unitless",
+        "year": 2030
+    },
+    "171-2030-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
         "maximum": 0.0384,
@@ -22891,23 +21925,23 @@
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "40t"
+            "32t"
         ],
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
-        "year": 2010
+        "year": 2030
     },
-    "1750-2020-combustion power share": {
+    "1710-2040-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -22919,17 +21953,17 @@
         "sizes": [
             "3.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2020
+        "year": 2040
     },
-    "1751-2030-combustion power share": {
+    "1711-2050-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -22941,61 +21975,61 @@
         "sizes": [
             "3.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2030
+        "year": 2050
     },
-    "1752-2040-combustion power share": {
+    "1712-2000-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
         "minimum": 0.65,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "3.5t"
+            "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2040
+        "year": 2000
     },
-    "1753-2050-combustion power share": {
+    "1713-2010-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
         "minimum": 0.65,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "3.5t"
+            "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2050
+        "year": 2010
     },
-    "1754-2000-combustion power share": {
+    "1714-2020-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -23007,17 +22041,17 @@
         "sizes": [
             "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2000
+        "year": 2020
     },
-    "1755-2010-combustion power share": {
+    "1715-2030-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -23029,17 +22063,17 @@
         "sizes": [
             "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2010
+        "year": 2030
     },
-    "1756-2020-combustion power share": {
+    "1716-2040-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -23051,17 +22085,17 @@
         "sizes": [
             "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2020
+        "year": 2040
     },
-    "1757-2030-combustion power share": {
+    "1717-2050-combustion power share": {
         "amount": 0.67,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.67,
         "maximum": 0.75,
@@ -23073,61 +22107,61 @@
         "sizes": [
             "7.5t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2030
+        "year": 2050
     },
-    "1758-2040-combustion power share": {
-        "amount": 0.67,
+    "1718-2000-combustion power share": {
+        "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.67,
+        "loc": 0.69,
         "maximum": 0.75,
         "minimum": 0.65,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "7.5t"
+            "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2040
+        "year": 2000
     },
-    "1759-2050-combustion power share": {
-        "amount": 0.67,
+    "1719-2010-combustion power share": {
+        "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.67,
+        "loc": 0.69,
         "maximum": 0.75,
         "minimum": 0.65,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "7.5t"
+            "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2050
+        "year": 2010
     },
-    "176-2020-toll cost per km": {
+    "172-2040-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
         "maximum": 0.0384,
@@ -23140,23 +22174,23 @@
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "40t"
+            "32t"
         ],
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
-        "year": 2020
+        "year": 2040
     },
-    "1760-2000-combustion power share": {
+    "1720-2020-combustion power share": {
         "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.69,
         "maximum": 0.75,
@@ -23168,17 +22202,17 @@
         "sizes": [
             "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2000
+        "year": 2020
     },
-    "1761-2010-combustion power share": {
+    "1721-2030-combustion power share": {
         "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.69,
         "maximum": 0.75,
@@ -23190,17 +22224,17 @@
         "sizes": [
             "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2010
+        "year": 2030
     },
-    "1762-2020-combustion power share": {
+    "1722-2040-combustion power share": {
         "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.69,
         "maximum": 0.75,
@@ -23212,17 +22246,17 @@
         "sizes": [
             "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2020
+        "year": 2040
     },
-    "1763-2030-combustion power share": {
+    "1723-2050-combustion power share": {
         "amount": 0.69,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.69,
         "maximum": 0.75,
@@ -23234,61 +22268,61 @@
         "sizes": [
             "18t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2030
+        "year": 2050
     },
-    "1764-2040-combustion power share": {
-        "amount": 0.69,
+    "1724-2000-combustion power share": {
+        "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.69,
-        "maximum": 0.75,
-        "minimum": 0.65,
+        "loc": 0.8,
+        "maximum": 0.85,
+        "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "18t"
+            "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2040
+        "year": 2000
     },
-    "1765-2050-combustion power share": {
-        "amount": 0.69,
+    "1725-2010-combustion power share": {
+        "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.69,
-        "maximum": 0.75,
-        "minimum": 0.65,
+        "loc": 0.8,
+        "maximum": 0.85,
+        "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "18t"
+            "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2050
+        "year": 2010
     },
-    "1766-2000-combustion power share": {
+    "1726-2020-combustion power share": {
         "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.8,
         "maximum": 0.85,
@@ -23300,17 +22334,17 @@
         "sizes": [
             "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2000
+        "year": 2020
     },
-    "1767-2010-combustion power share": {
+    "1727-2030-combustion power share": {
         "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.8,
         "maximum": 0.85,
@@ -23322,17 +22356,17 @@
         "sizes": [
             "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2010
+        "year": 2030
     },
-    "1768-2020-combustion power share": {
+    "1728-2040-combustion power share": {
         "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.8,
         "maximum": 0.85,
@@ -23344,17 +22378,17 @@
         "sizes": [
             "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2020
+        "year": 2040
     },
-    "1769-2030-combustion power share": {
+    "1729-2050-combustion power share": {
         "amount": 0.8,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.8,
         "maximum": 0.85,
@@ -23366,17 +22400,17 @@
         "sizes": [
             "26t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2030
+        "year": 2050
     },
-    "177-2030-toll cost per km": {
+    "173-2050-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
         "maximum": 0.0384,
@@ -23389,67 +22423,67 @@
             "ICEV-g",
             "BEV",
             "FCEV",
             "HEV-d",
             "PHEV-d"
         ],
         "sizes": [
-            "40t"
+            "32t"
         ],
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
-        "year": 2030
+        "year": 2050
     },
-    "1770-2040-combustion power share": {
-        "amount": 0.8,
+    "1730-2000-combustion power share": {
+        "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.8,
-        "maximum": 0.85,
+        "loc": 0.775,
+        "maximum": 0.8,
         "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "26t"
+            "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2040
+        "year": 2000
     },
-    "1771-2050-combustion power share": {
-        "amount": 0.8,
+    "1731-2010-combustion power share": {
+        "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.8,
-        "maximum": 0.85,
+        "loc": 0.775,
+        "maximum": 0.8,
         "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "26t"
+            "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2050
+        "year": 2010
     },
-    "1772-2000-combustion power share": {
+    "1732-2020-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23461,17 +22495,17 @@
         "sizes": [
             "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2000
+        "year": 2020
     },
-    "1773-2010-combustion power share": {
+    "1733-2030-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23483,17 +22517,17 @@
         "sizes": [
             "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2010
+        "year": 2030
     },
-    "1774-2020-combustion power share": {
+    "1734-2040-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23505,17 +22539,17 @@
         "sizes": [
             "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2020
+        "year": 2040
     },
-    "1775-2030-combustion power share": {
+    "1735-2050-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23527,61 +22561,61 @@
         "sizes": [
             "32t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2030
+        "year": 2050
     },
-    "1776-2040-combustion power share": {
+    "1736-2000-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
         "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "32t"
+            "40t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2040
+        "year": 2000
     },
-    "1777-2050-combustion power share": {
+    "1737-2010-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
         "minimum": 0.75,
         "name": "combustion power share",
         "powertrain": [
             "HEV-d"
         ],
         "sizes": [
-            "32t"
+            "40t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2050
+        "year": 2010
     },
-    "1778-2000-combustion power share": {
+    "1738-2020-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23593,17 +22627,17 @@
         "sizes": [
             "40t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2000
+        "year": 2020
     },
-    "1779-2010-combustion power share": {
+    "1739-2030-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23615,17 +22649,17 @@
         "sizes": [
             "40t"
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
-        "year": 2010
+        "year": 2030
     },
-    "178-2040-toll cost per km": {
+    "174-2000-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
         "maximum": 0.0384,
@@ -23644,61 +22678,17 @@
         "sizes": [
             "40t"
         ],
         "source": "TRACCS https://traccs.emisia.com/index.php",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "\u20ac/km",
-        "year": 2040
-    },
-    "1780-2020-combustion power share": {
-        "amount": 0.775,
-        "category": "Powertrain",
-        "comment": "Based on US trucks",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.775,
-        "maximum": 0.8,
-        "minimum": 0.75,
-        "name": "combustion power share",
-        "powertrain": [
-            "HEV-d"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2020
-    },
-    "1781-2030-combustion power share": {
-        "amount": 0.775,
-        "category": "Powertrain",
-        "comment": "Based on US trucks",
-        "importance": "Critical",
-        "kind": "distribution",
-        "loc": 0.775,
-        "maximum": 0.8,
-        "minimum": 0.75,
-        "name": "combustion power share",
-        "powertrain": [
-            "HEV-d"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "unitless",
-        "year": 2030
+        "year": 2000
     },
-    "1782-2040-combustion power share": {
+    "1740-2040-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23712,15 +22702,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1783-2050-combustion power share": {
+    "1741-2050-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23734,15 +22724,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "1784-2000-combustion power share": {
+    "1742-2000-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23756,15 +22746,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2000
     },
-    "1785-2010-combustion power share": {
+    "1743-2010-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23778,15 +22768,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2010
     },
-    "1786-2020-combustion power share": {
+    "1744-2020-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23800,15 +22790,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2020
     },
-    "1787-2030-combustion power share": {
+    "1745-2030-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23822,15 +22812,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2030
     },
-    "1788-2040-combustion power share": {
+    "1746-2040-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23844,15 +22834,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2040
     },
-    "1789-2050-combustion power share": {
+    "1747-2050-combustion power share": {
         "amount": 0.775,
         "category": "Powertrain",
         "comment": "Based on US trucks",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.775,
         "maximum": 0.8,
@@ -23866,44 +22856,15 @@
         ],
         "source": "https://www.mdpi.com/2032-6653/11/1/12/pdf",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "unitless",
         "year": 2050
     },
-    "179-2050-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "40t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2050
-    },
-    "1790-2000-combustion power share": {
+    "1748-2000-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -23922,15 +22883,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2000
     },
-    "1791-2010-combustion power share": {
+    "1749-2010-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -23949,15 +22910,44 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2010
     },
-    "1792-2020-combustion power share": {
+    "175-2010-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "40t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2010
+    },
+    "1750-2020-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -23976,15 +22966,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2020
     },
-    "1793-2030-combustion power share": {
+    "1751-2030-combustion power share": {
         "amount": 0.95,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.95,
         "name": "combustion power share",
@@ -24003,15 +22993,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2030
     },
-    "1794-2040-combustion power share": {
+    "1752-2040-combustion power share": {
         "amount": 0.9,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.9,
         "name": "combustion power share",
@@ -24030,15 +23020,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2040
     },
-    "1795-2050-combustion power share": {
+    "1753-2050-combustion power share": {
         "amount": 0.85,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0.85,
         "name": "combustion power share",
@@ -24057,15 +23047,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2050
     },
-    "1796-2000-combustion power share": {
+    "1754-2000-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24083,15 +23073,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2000
     },
-    "1797-2010-combustion power share": {
+    "1755-2010-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24109,15 +23099,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2010
     },
-    "1798-2020-combustion power share": {
+    "1756-2020-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24135,15 +23125,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2020
     },
-    "1799-2030-combustion power share": {
+    "1757-2030-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24161,73 +23151,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2030
     },
-    "18-2000-heating thermal demand": {
-        "amount": 325,
-        "category": "Auxiliaries",
-        "comment": "own assumption",
-        "importance": "Limited",
-        "kind": "distribution",
-        "loc": 325,
-        "maximum": 390,
-        "minimum": 260,
-        "name": "heating thermal demand",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "26t"
-        ],
-        "source": "",
-        "status": "To be improved",
-        "uncertainty_type": 5,
-        "unit": "W",
-        "year": 2000
-    },
-    "180-2000-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2000
-    },
-    "1800-2040-combustion power share": {
+    "1758-2040-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24245,15 +23177,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2040
     },
-    "1801-2050-combustion power share": {
+    "1759-2050-combustion power share": {
         "amount": 1,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 1,
         "name": "combustion power share",
@@ -24271,15 +23203,44 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2050
     },
-    "1802-2000-combustion power share": {
+    "176-2020-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "40t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2020
+    },
+    "1760-2000-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24299,15 +23260,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2000
     },
-    "1803-2010-combustion power share": {
+    "1761-2010-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24327,15 +23288,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2010
     },
-    "1804-2020-combustion power share": {
+    "1762-2020-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24355,15 +23316,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2020
     },
-    "1805-2030-combustion power share": {
+    "1763-2030-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24383,15 +23344,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2030
     },
-    "1806-2040-combustion power share": {
+    "1764-2040-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24411,15 +23372,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2040
     },
-    "1807-2050-combustion power share": {
+    "1765-2050-combustion power share": {
         "amount": 0,
         "category": "Powertrain",
         "comment": "Same as for passenger vehicles.",
         "importance": "Critical",
         "kind": "distribution",
         "loc": 0,
         "name": "combustion power share",
@@ -24439,15 +23400,15 @@
         ],
         "source": "Cox et al. 2020",
         "status": "Good",
         "uncertainty_type": 1,
         "unit": "unitless",
         "year": 2050
     },
-    "1808-2000-charger mass": {
+    "1766-2000-charger mass": {
         "amount": 39.690000000000005,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 39.690000000000005,
         "maximum": 44.1,
@@ -24468,15 +23429,15 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2000
     },
-    "1809-2010-charger mass": {
+    "1767-2010-charger mass": {
         "amount": 37.800000000000004,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 37.800000000000004,
         "maximum": 42,
@@ -24497,44 +23458,15 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2010
     },
-    "181-2010-toll cost per km": {
-        "amount": 0.032,
-        "category": "Costs",
-        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
-        "importance": "Unknown",
-        "kind": "distribution",
-        "loc": 0.032,
-        "maximum": 0.0384,
-        "minimum": 0.0256,
-        "name": "toll cost per km",
-        "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
-            "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
-        ],
-        "sizes": [
-            "60t"
-        ],
-        "source": "TRACCS https://traccs.emisia.com/index.php",
-        "status": "Acceptable",
-        "uncertainty_type": 5,
-        "unit": "\u20ac/km",
-        "year": 2010
-    },
-    "1810-2020-charger mass": {
+    "1768-2020-charger mass": {
         "amount": 36,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 36,
         "maximum": 40,
@@ -24555,15 +23487,15 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2020
     },
-    "1811-2030-charger mass": {
+    "1769-2030-charger mass": {
         "amount": 36,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 36,
         "maximum": 40,
@@ -24584,15 +23516,44 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2030
     },
-    "1812-2040-charger mass": {
+    "177-2030-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "40t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2030
+    },
+    "1770-2040-charger mass": {
         "amount": 34.199999999999996,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 34.199999999999996,
         "maximum": 40,
@@ -24613,15 +23574,15 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2040
     },
-    "1813-2050-charger mass": {
+    "1771-2050-charger mass": {
         "amount": 32.489999999999995,
         "category": "Powertrain",
         "comment": "Assumes three 22kW chargers connected in parallel, to charge a 1000 kWh battery in 16 hours.",
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 32.489999999999995,
         "maximum": 38,
@@ -24642,14 +23603,651 @@
         ],
         "source": "Brusa, https://www.brusa.biz/fileadmin/template/Support-Center/Datenbl%C3%A4tter/BRUSA_DB_EN_NLG664.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kg",
         "year": 2050
     },
+    "1772-2000-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2000
+    },
+    "1773-2010-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2010
+    },
+    "1774-2020-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2020
+    },
+    "1775-2030-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2030
+    },
+    "1776-2040-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2040
+    },
+    "1777-2050-battery charge efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Same as for passenger vehicles.",
+        "importance": "Moderate",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "battery charge efficiency",
+        "powertrain": [
+            "ICEV-d",
+            "HEV-d",
+            "ICEV-g",
+            "PHEV-c-d"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "Cox et al. 2020",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2050
+    },
+    "1778-2000-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2000
+    },
+    "1779-2010-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2010
+    },
+    "178-2040-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "40t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2040
+    },
+    "1780-2020-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2020
+    },
+    "1781-2030-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2030
+    },
+    "1782-2040-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2040
+    },
+    "1783-2050-charger efficiency": {
+        "amount": 1,
+        "category": "Energy Storage",
+        "comment": "Not used.",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 1,
+        "name": "charger efficiency",
+        "powertrain": [
+            "BEV",
+            "PHEV-e"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "unitless",
+        "year": 2050
+    },
+    "1784-2000-fuel cell power density": {
+        "amount": 1.1,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 1.1,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2000
+    },
+    "1785-2010-fuel cell power density": {
+        "amount": 1.05,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 1.05,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2010
+    },
+    "1786-2020-fuel cell power density": {
+        "amount": 1.02,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 1.02,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2020
+    },
+    "1787-2030-fuel cell power density": {
+        "amount": 0.93,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 0.93,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2030
+    },
+    "1788-2040-fuel cell power density": {
+        "amount": 0.8400000000000001,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 0.8400000000000001,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2040
+    },
+    "1789-2050-fuel cell power density": {
+        "amount": 0.7407407407407407,
+        "category": "Powertrain",
+        "comment": "U.S DoE \"ultimate target\" considered to be 2050. Power density for buses and trucks assumed to be twice as large than for passenger cars (0.51).",
+        "importance": "Critical",
+        "kind": "distribution",
+        "loc": 0.7407407407407407,
+        "name": "fuel cell power density",
+        "powertrain": [
+            "FCEV"
+        ],
+        "sizes": [
+            "3.5t",
+            "7.5t",
+            "18t",
+            "26t",
+            "32t",
+            "40t",
+            "60t"
+        ],
+        "source": "https://www.hydrogen.energy.gov/pdfs/20005-automotive-fuel-cell-targets-status.pdf",
+        "status": "Acceptable",
+        "uncertainty_type": 1,
+        "unit": "kg/kW",
+        "year": 2050
+    },
+    "179-2050-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "40t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2050
+    },
+    "18-2000-heating thermal demand": {
+        "amount": 325,
+        "category": "Auxiliaries",
+        "comment": "own assumption",
+        "importance": "Limited",
+        "kind": "distribution",
+        "loc": 325,
+        "maximum": 390,
+        "minimum": 260,
+        "name": "heating thermal demand",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "26t"
+        ],
+        "source": "",
+        "status": "To be improved",
+        "uncertainty_type": 5,
+        "unit": "W",
+        "year": 2000
+    },
+    "180-2000-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "60t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2000
+    },
+    "181-2010-toll cost per km": {
+        "amount": 0.032,
+        "category": "Costs",
+        "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
+        "importance": "Unknown",
+        "kind": "distribution",
+        "loc": 0.032,
+        "maximum": 0.0384,
+        "minimum": 0.0256,
+        "name": "toll cost per km",
+        "powertrain": [
+            "PHEV-c-d",
+            "PHEV-e",
+            "ICEV-d",
+            "ICEV-g",
+            "BEV",
+            "FCEV",
+            "HEV-d",
+            "PHEV-d"
+        ],
+        "sizes": [
+            "60t"
+        ],
+        "source": "TRACCS https://traccs.emisia.com/index.php",
+        "status": "Acceptable",
+        "uncertainty_type": 5,
+        "unit": "\u20ac/km",
+        "year": 2010
+    },
     "182-2020-toll cost per km": {
         "amount": 0.032,
         "category": "Costs",
         "comment": "Toll cost for BEVs and FCEVs assumed similar to ICEV-d. Representative of Switzerland.",
         "importance": "Unknown",
         "kind": "distribution",
         "loc": 0.032,
@@ -40581,22 +40179,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.85,
         "maximum": 0.9,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -40616,22 +40209,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.85,
         "maximum": 0.9,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -40709,22 +40297,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.85,
         "maximum": 0.9,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -40744,22 +40327,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.85,
         "maximum": 0.9,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -40779,22 +40357,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.8627499999999999,
         "maximum": 0.927,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -40814,22 +40387,17 @@
         "importance": "Moderate",
         "kind": "distribution",
         "loc": 0.8627499999999999,
         "maximum": 0.927,
         "minimum": 0.8,
         "name": "battery charge efficiency",
         "powertrain": [
-            "PHEV-c-d",
-            "PHEV-e",
-            "ICEV-d",
-            "ICEV-g",
             "BEV",
-            "FCEV",
-            "HEV-d",
-            "PHEV-d"
+            "PHEV-e",
+            "FCEV"
         ],
         "sizes": [
             "3.5t",
             "7.5t",
             "18t",
             "26t",
             "32t",
@@ -44742,22 +44310,22 @@
         "source": "",
         "status": "To be improved",
         "uncertainty_type": 5,
         "unit": "W",
         "year": 2040
     },
     "820-2020-battery cell energy density, LFP": {
-        "amount": 0.19999999999999998,
+        "amount": 0.15,
         "category": "Energy Storage",
         "comment": "",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.19999999999999998,
-        "maximum": 0.24999999999999997,
-        "minimum": 0.15,
+        "loc": 0.15,
+        "maximum": 0.1875,
+        "minimum": 0.11249999999999999,
         "name": "battery cell energy density, LFP",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -44777,22 +44345,22 @@
         "source": "https://pubs.acs.org/doi/pdf/10.1021/acsenergylett.7b00432\nhttps://theicct.org/wp-content/uploads/2021/12/eu-tractor-trailers-analysis-aug21-2.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kWh/kg",
         "year": 2020
     },
     "821-2030-battery cell energy density, LFP": {
-        "amount": 0.26,
+        "amount": 0.2,
         "category": "Energy Storage",
         "comment": "",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.26,
-        "maximum": 0.325,
-        "minimum": 0.195,
+        "loc": 0.2,
+        "maximum": 0.25,
+        "minimum": 0.15000000000000002,
         "name": "battery cell energy density, LFP",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
@@ -44812,22 +44380,22 @@
         "source": "https://pubs.acs.org/doi/pdf/10.1021/acsenergylett.7b00432\nhttps://theicct.org/wp-content/uploads/2021/12/eu-tractor-trailers-analysis-aug21-2.pdf",
         "status": "Acceptable",
         "uncertainty_type": 5,
         "unit": "kWh/kg",
         "year": 2030
     },
     "822-2040-battery cell energy density, LFP": {
-        "amount": 0.3,
+        "amount": 0.25,
         "category": "Energy Storage",
         "comment": "",
         "importance": "Critical",
         "kind": "distribution",
-        "loc": 0.3,
-        "maximum": 0.375,
-        "minimum": 0.22499999999999998,
+        "loc": 0.25,
+        "maximum": 0.3125,
+        "minimum": 0.1875,
         "name": "battery cell energy density, LFP",
         "powertrain": [
             "PHEV-c-d",
             "PHEV-e",
             "ICEV-d",
             "ICEV-g",
             "BEV",
```

### Comparing `carculator_truck-0.3.8/carculator_truck/data/extra_parameters.json` & `carculator_truck-0.3.9/carculator_truck/data/extra_parameters.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9498207885304659%*

 * *Differences: {'delete': '[95, 70, 54, 49, 26, 14]',*

 * * 'insert': "[(25, 'Non-methane hydrocarbon direct emissions, rural'), (48, 'Non-methane "*

 * *           "hydrocarbon direct emissions, urban'), (53, 'Non-methane hydrocarbon direct emissions, "*

 * *           "suburban'), (268, 'fuel density per kg'), (269, 'fuel consumption'), (270, 'Nitrogen "*

 * *           "dioxide direct emissions, rural'), (271, 'Nitrogen dioxide direct emissions, "*

 * *           "suburban'), (272, 'Nitrogen dioxide direct emissions, urban')]"}*

```diff
@@ -9,27 +9,26 @@
     "Ammonia direct emissions, rural",
     "curb mass",
     "Nitrogen oxides direct emissions, rural",
     "noise, octave 7, evening time, rural",
     "noise, octave 1, night time, suburban",
     "noise, octave 3, evening time, rural",
     "TtW energy",
-    "Sulfur dioxide direct emissions, rural",
     "noise, octave 3, day time, urban",
     "noise, octave 2, day time, rural",
     "battery power",
     "amortised purchase cost",
     "noise, octave 1, day time, suburban",
     "Dinitrogen oxide direct emissions, urban",
     "battery cell production heat",
     "noise, octave 8, evening time, suburban",
     "noise, octave 3, day time, rural",
     "noise, octave 4, day time, urban",
     "fuel cell system efficiency",
-    "NMVOC direct emissions, rural",
+    "Non-methane hydrocarbon direct emissions, rural",
     "noise, octave 3, night time, suburban",
     "total cost per km",
     "energy cost",
     "electric engine mass",
     "Methane direct emissions, suburban",
     "Carbon monoxide direct emissions, rural",
     "Particulate matters direct emissions, urban",
@@ -44,20 +43,20 @@
     "Nitrogen oxides direct emissions, urban",
     "noise, octave 3, evening time, urban",
     "noise, octave 4, night time, rural",
     "noise, octave 8, evening time, rural",
     "fuel cell essential BoP mass",
     "noise, octave 3, day time, suburban",
     "electric powertrain cost",
-    "NMVOC direct emissions, urban",
+    "Non-methane hydrocarbon direct emissions, urban",
     "noise, octave 2, day time, urban",
     "noise, octave 6, day time, rural",
     "noise, octave 5, day time, urban",
     "noise, octave 1, evening time, rural",
-    "NMVOC direct emissions, suburban",
+    "Non-methane hydrocarbon direct emissions, suburban",
     "noise, octave 7, night time, urban",
     "Methane direct emissions, rural",
     "noise, octave 5, day time, suburban",
     "noise, octave 2, night time, rural",
     "fuel cell power",
     "noise, octave 7, night time, rural",
     "TtW efficiency",
@@ -65,15 +64,14 @@
     "noise, octave 6, night time, urban",
     "energy battery cost",
     "fuel tank mass",
     "Ammonia direct emissions, suburban",
     "auxiliary power demand",
     "glider cost",
     "Benzene direct emissions, rural",
-    "Sulfur dioxide direct emissions, suburban",
     "noise, octave 7, day time, urban",
     "Methane direct emissions, urban",
     "noise, octave 3, night time, rural",
     "noise, octave 5, night time, urban",
     "Hydrocarbons direct emissions, rural",
     "combustion powertrain cost",
     "noise, octave 8, day time, suburban",
@@ -90,15 +88,14 @@
     "noise, octave 6, evening time, rural",
     "electricity consumption",
     "power",
     "Lead direct emissions, urban",
     "noise, octave 1, evening time, urban",
     "oxidation energy stored",
     "noise, octave 2, evening time, suburban",
-    "Sulfur dioxide direct emissions, urban",
     "noise, octave 4, day time, suburban",
     "noise, octave 8, night time, suburban",
     "recuperation efficiency",
     "noise, octave 8, night time, rural",
     "noise, octave 2, night time, suburban",
     "combustion power",
     "noise, octave 4, night time, urban",
@@ -265,9 +262,14 @@
     "battery cell energy density",
     "battery cell mass share",
     "battery cycle life",
     "total cargo mass",
     "cargo mass",
     "kilometers per year",
     "TtW energy, combustion mode",
-    "TtW energy, electric mode"
+    "TtW energy, electric mode",
+    "fuel density per kg",
+    "fuel consumption",
+    "Nitrogen dioxide direct emissions, rural",
+    "Nitrogen dioxide direct emissions, suburban",
+    "Nitrogen dioxide direct emissions, urban"
 ]
```

### Comparing `carculator_truck-0.3.8/carculator_truck/data/payloads.yaml` & `carculator_truck-0.3.9/carculator_truck/data/payloads.yaml`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.8/carculator_truck.egg-info/PKG-INFO` & `carculator_truck-0.3.9/carculator_truck.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator-truck
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prospective environmental and economic life cycle assessmentof medium and heavy goods vehicles
 Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -51,15 +51,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ``carculator_truck``
 
 <p align="center">
-  <img style="height:130px;" src="https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png">
+  <img style="height:130px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/mediumsmall.png">
 </p>
 
 
 <p align="center">
   <a href="https://badge.fury.io/py/carculator-truck" target="_blank"><img src="https://badge.fury.io/py/carculator-truck.svg"></a>
   <a href="https://github.com/romainsacchi/carculator_truck" target="_blank"><img src="https://github.com/romainsacchi/carculator_truck/actions/workflows/main.yml/badge.svg?branch=master"></a>
   <a href="https://coveralls.io/github/romainsacchi/carculator_truck" target="_blank"><img src="https://coveralls.io/repos/github/romainsacchi/carculator_truck/badge.svg"></a>
@@ -105,33 +105,37 @@
 <a href="https://www.simapro.com/" target="_blank">SimaPro 9.x.</a>.</li>
 </ul>
 
 <p align="center">
     The energy model of <i>carculator_truck</i> considers the vehicle aerodynamics, the road gradient and other factors.
     It also considers varying efficiencies of the transmission and engine at various load points for each second
     of the driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/energy_model.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/energy_model.png">
 </p>
 
 <p align="center">
     The energy model and the calculated tank-to-wheel energy consumption is validated against the simulation software
     <a href="https://ec.europa.eu/clima/policies/transport/vehicles/vecto_en" target="_blank">VECTO</a>.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/vecto_validation.png">
 </p>
 
 <p align="center">
     Benefits of hybrid powertrains are fully conidered: the possibility to recuperate braking energy as well as efficiency gains from engine
     downsizing is accounted for.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/hybrid_efficiency.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/hybrid_efficiency.png">
 </p>
 
 <p align="center">
     Global warming potential impacts per ton-km for a 40-t truck, across different powertrain technologies,
     using an urban driving cycle.
-  <img style="height:50px;" src="https://github.com/romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png">
+  
+  <img style="height:150px;" src="https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png">
 </p>
 
 ## How to use it?
 
 See the notebook with [examples](https://github.com/romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb).
 
 ## Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator-truck Version: 0.3.8 Summary:
+Metadata-Version: 2.1 Name: carculator-truck Version: 0.3.9 Summary:
 Prospective environmental and economic life cycle assessmentof medium and heavy
 goods vehicles Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi
 sacchi@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
@@ -30,15 +30,16 @@
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Mathematics Classifier: Topic :: Scientific/Engineering ::
 Visualization Description-Content-Type: text/markdown License-File: LICENSE #
 ``carculator_truck``
-   [https://github.com/romainsacchi/coarse/raw/master/docs/mediumsmall.png]
+[https://github.com/romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                               mediumsmall.png]
      [https://badge.fury.io/py/carculator-truck.svg] [https://github.com/
            romainsacchi/carculator_truck/actions/workflows/main.yml/
    badge.svg?branch=master] [https://coveralls.io/repos/github/romainsacchi/
 carculator_truck/badge.svg] [https://readthedocs.org/projects/carculator_truck/
                             badge/?version=latest]
 Prospective environmental and economic life cycle assessment of medium and
 heavy duty vehicles. A fully parameterized Python model developed by the
@@ -67,26 +68,27 @@
       level but also in the rest of the world energy system (e.g., power
       generation) is accounted for, using energy scenario-specific IAM-coupled
       ecoinvent databases produced by premise.
     * Inventories can be imported into Brightway2 and SimaPro_9.x..
  The energy model of carculator_truck considers the vehicle aerodynamics, the
 road gradient and other factors. It also considers varying efficiencies of the
  transmission and engine at various load points for each second of the driving
-   cycle. [https://github.com/romainsacchi/carculator_truck/raw/master/docs/
-                               energy_model.png]
+  cycle. [https://github.com/romainsacchi/carculator_truck/blob/master/docs/
+                         _static/img/energy_model.png]
     The energy model and the calculated tank-to-wheel energy consumption is
      validated against the simulation software VECTO. [https://github.com/
-      romainsacchi/carculator_truck/raw/master/docs/vecto_validation.png]
+          romainsacchi/carculator_truck/blob/master/docs/_static/img/
+                             vecto_validation.png]
     Benefits of hybrid powertrains are fully conidered: the possibility to
 recuperate braking energy as well as efficiency gains from engine downsizing is
- accounted for. [https://github.com/romainsacchi/carculator_truck/raw/master/
-                          docs/hybrid_efficiency.png]
+ accounted for. [https://github.com/romainsacchi/carculator_truck/blob/master/
+                    docs/_static/img/hybrid_efficiency.png]
 Global warming potential impacts per ton-km for a 40-t truck, across different
   powertrain technologies, using an urban driving cycle. [https://github.com/
-         romainsacchi/carculator_truck/raw/master/docs/urban_gwp.png]
+   romainsacchi/carculator_truck/blob/master/docs/_static/img/urban_gwp.png]
 ## How to use it? See the notebook with [examples](https://github.com/
 romainsacchi/carculator_truck/blob/master/examples/Examples.ipynb). ## Support
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:
 carculator@psi.ch). ## Maintainers * [Romain Sacchi](https://github.com/
 romainsacchi) * [Chris Mutel](https://github.com/cmutel/) ## Contributing See
 [contributing](https://github.com/romainsacchi/carculator_truck/blob/master/
 CONTRIBUTING.md). ## License [BSD-3-Clause](https://github.com/romainsacchi/
```

### Comparing `carculator_truck-0.3.8/setup.py` & `carculator_truck-0.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,42 +21,30 @@
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 
 def package_files(directory):
     paths = []
-    for (path, directories, filenames) in os.walk(directory):
+    for path, directories, filenames in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 setup(
     name="carculator_truck",
-    version="0.3.8",
+    version="0.3.9",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     package_data={
         "carculator_truck": package_files(os.path.join("carculator_truck", "data"))
     },
-    install_requires=[
-        "pandas",
-        "xarray",
-        "numpy",
-        "klausen",
-        "xlrd",
-        "numexpr",
-        "bw2io",
-        "prettytable",
-        "wurst",
-        "pycountry",
-        "pyyaml",
-    ],
+    install_requires=["carculator_utils", "prettytable"],
     url="https://github.com/romainsacchi/carculator_truck",
     description="Prospective environmental and economic life cycle assessment"
     "of medium and heavy goods vehicles",
     long_description_content_type="text/markdown",
     long_description=README,
     classifiers=[
         "Intended Audience :: End Users/Desktop",
```


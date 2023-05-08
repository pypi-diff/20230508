# Comparing `tmp/dtscalibration-1.1.2.tar.gz` & `tmp/dtscalibration-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtscalibration-1.1.2.tar", last modified: Sun Sep 25 16:03:34 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dtscalibration-1.1.2.tar` & `dtscalibration-1.2.0.tar`

### file list

```diff
@@ -1,232 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.502999 dtscalibration-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.462996 dtscalibration-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.466996 dtscalibration-1.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8147 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9691 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13376 2022-09-25 16:03:34.502999 dtscalibration-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.466996 dtscalibration-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.DataStore.rst
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.check_dims.rst
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.check_timestep_allclose.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.get_netcdf_encoding.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.merge_double_ended.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.open_datastore.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.open_mf_datastore.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.plot_accuracy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.plot_location_residuals_double_ended.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.plot_residuals_reference_sections.rst
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.plot_residuals_reference_sections_single.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.plot_sigma_report.rst
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.read_apsensing_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.read_sensornet_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.read_sensortran_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.read_silixa_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.shift_double_ended.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/api/dtscalibration.suggest_cable_shift_double_ended.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)     6330 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/01Load_xml_measurement_files.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)    24566 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/03Define_sections.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/04Calculate_variance_Stokes.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/04Calculate_variance_Stokes.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    20652 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/04Calculate_variance_Stokes.ipynb_files/04Calculate_variance_Stokes.ipynb_11_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    30156 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/04Calculate_variance_Stokes.ipynb_files/04Calculate_variance_Stokes.ipynb_9_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    11048 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/05Calibrate_single_ols.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/05Calibrate_single_ols.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    45597 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/05Calibrate_single_ols.ipynb_files/05Calibrate_single_ols.ipynb_7_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    17552 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/06Calibrate_double_ols.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/06Calibrate_double_ols.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    55762 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/06Calibrate_double_ols.ipynb_files/06Calibrate_double_ols.ipynb_7_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    36519 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/06Calibrate_double_ols.ipynb_files/06Calibrate_double_ols.ipynb_9_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    50177 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/07Calibrate_single_wls.ipynb_11_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    19693 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/07Calibrate_single_wls.ipynb_12_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    47096 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/07Calibrate_single_wls.ipynb_13_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    38293 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/07Calibrate_single_wls.ipynb_15_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    30250 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/07Calibrate_single_wls.ipynb_files/07Calibrate_single_wls.ipynb_17_0.png
--rw-r--r--   0 runner    (1001) docker     (121)     5965 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    58936 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb_files/08Calibrate_double_wls.ipynb_13_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    56022 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb_files/08Calibrate_double_wls.ipynb_15_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    17609 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb_files/08Calibrate_double_wls.ipynb_6_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    12663 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/08Calibrate_double_wls.ipynb_files/08Calibrate_double_wls.ipynb_9_1.png
--rw-r--r--   0 runner    (1001) docker     (121)     5438 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/09Import_timeseries.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/10Align_double_ended_measurements.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.470996 dtscalibration-1.1.2/docs/examples/notebooks/10Align_double_ended_measurements.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    48488 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/10Align_double_ended_measurements.ipynb_files/10Align_double_ended_measurements.ipynb_8_1.png
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/11Merge_single_measurements_into_double.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/examples/notebooks/11Merge_single_measurements_into_double.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    24572 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/11Merge_single_measurements_into_double.ipynb_files/11Merge_single_measurements_into_double.ipynb_10_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    17407 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/11Merge_single_measurements_into_double.ipynb_files/11Merge_single_measurements_into_double.ipynb_6_1.png
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/12Datastore_from_numpy_arrays.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/13Fixed_parameter_calibration.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/examples/notebooks/13Fixed_parameter_calibration.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    45469 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/13Fixed_parameter_calibration.ipynb_files/13Fixed_parameter_calibration.ipynb_7_0.png
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/14Lossy_splices.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/examples/notebooks/14Lossy_splices.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    24217 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/14Lossy_splices.ipynb_files/14Lossy_splices.ipynb_11_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    25591 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/14Lossy_splices.ipynb_files/14Lossy_splices.ipynb_7_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    16322 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/14Lossy_splices.ipynb_files/14Lossy_splices.ipynb_9_1.png
--rw-r--r--   0 runner    (1001) docker     (121)     5619 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/15Matching_sections.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/examples/notebooks/15Matching_sections.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    23046 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/15Matching_sections.ipynb_files/15Matching_sections.ipynb_10_2.png
--rw-r--r--   0 runner    (1001) docker     (121)    16582 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/15Matching_sections.ipynb_files/15Matching_sections.ipynb_8_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    11937 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb_files/
--rw-r--r--   0 runner    (1001) docker     (121)    20580 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb_files/16Averaging_temperatures.ipynb_10_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    17803 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb_files/16Averaging_temperatures.ipynb_13_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    10368 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb_files/16Averaging_temperatures.ipynb_16_0.png
--rw-r--r--   0 runner    (1001) docker     (121)    15790 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/16Averaging_temperatures.ipynb_files/16Averaging_temperatures.ipynb_19_0.png
--rw-r--r--   0 runner    (1001) docker     (121)     7441 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/A2Load_sensornet_files.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/A3Load_ap_sensing_files.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)    36247 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/examples/notebooks/A4Load_sensortran_files.ipynb.rst
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/nb_examples_to_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-25 16:03:34.502999 dtscalibration-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.462996 dtscalibration-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.474997 dtscalibration-1.1.2/src/dtscalibration/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51325 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/calibrate_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)   241204 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/datastore.py
--rw-r--r--   0 runner    (1001) docker     (121)    12525 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/datastore_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    60445 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/io.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24384 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/src/dtscalibration/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.478997 dtscalibration-1.1.2/src/dtscalibration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13376 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10550 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-25 16:03:34.000000 dtscalibration-1.1.2/src/dtscalibration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.478997 dtscalibration-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.462996 dtscalibration-1.1.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.478997 dtscalibration-1.1.2/tests/data/ap_sensing/
--rw-r--r--   0 runner    (1001) docker     (121)   677982 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
--rw-r--r--   0 runner    (1001) docker     (121)   678035 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
--rw-r--r--   0 runner    (1001) docker     (121)   678009 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.482997 dtscalibration-1.1.2/tests/data/double_ended/
--rwxr-xr-x   0 runner    (1001) docker     (121)   171342 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921112245510.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   171341 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921112746818.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   171310 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921113248085.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.482997 dtscalibration-1.1.2/tests/data/double_ended2/
--rwxr-xr-x   0 runner    (1001) docker     (121)   129624 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014052498.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   129585 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014057119.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   129431 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014101652.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   129452 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014106243.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   129559 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014110917.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)   129482 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014115480.xml
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_ended2/info.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.462996 dtscalibration-1.1.2/tests/data/double_single_ended/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.486998 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/
--rw-r--r--   0 runner    (1001) docker     (121)   436539 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436736 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436525 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436669 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436527 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436478 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.490998 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/
--rw-r--r--   0 runner    (1001) docker     (121)   436371 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436475 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436421 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436359 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436400 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
--rw-r--r--   0 runner    (1001) docker     (121)   436238 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.490998 dtscalibration-1.1.2/tests/data/external_temperature_timeseries/
--rwxr-xr-x   0 runner    (1001) docker     (121)    20057 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
--rwxr-xr-x   0 runner    (1001) docker     (121)    20028 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
--rwxr-xr-x   0 runner    (1001) docker     (121)    20086 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.490998 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    47136 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    47126 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    47113 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    47107 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    47100 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.490998 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/
--rw-r--r--   0 runner    (1001) docker     (121)    64983 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65031 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65017 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65058 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65029 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65043 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    65018 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.494999 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/
--rw-r--r--   0 runner    (1001) docker     (121)    48160 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    48206 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    48196 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    48174 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)    48163 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.494999 dtscalibration-1.1.2/tests/data/sensornet_sentinel_v5.1_double/
--rw-r--r--   0 runner    (1001) docker     (121)   126331 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
--rw-r--r--   0 runner    (1001) docker     (121)   126323 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.494999 dtscalibration-1.1.2/tests/data/sensortran_binary/
--rw-r--r--   0 runner    (1001) docker     (121)    96176 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
--rw-r--r--   0 runner    (1001) docker     (121)    92832 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
--rw-r--r--   0 runner    (1001) docker     (121)    96176 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
--rw-r--r--   0 runner    (1001) docker     (121)    92832 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
--rw-r--r--   0 runner    (1001) docker     (121)    96176 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
--rw-r--r--   0 runner    (1001) docker     (121)    92832 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.498999 dtscalibration-1.1.2/tests/data/silixa_v4.5/
--rw-r--r--   0 runner    (1001) docker     (121)   164764 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164730 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164757 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164679 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164785 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164691 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
--rw-r--r--   0 runner    (1001) docker     (121)   164784 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.498999 dtscalibration-1.1.2/tests/data/silixa_v7.0/
--rw-r--r--   0 runner    (1001) docker     (121)   215137 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
--rw-r--r--   0 runner    (1001) docker     (121)   215082 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
--rw-r--r--   0 runner    (1001) docker     (121)   215091 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
--rw-r--r--   0 runner    (1001) docker     (121)   215114 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
--rw-r--r--   0 runner    (1001) docker     (121)   215119 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.498999 dtscalibration-1.1.2/tests/data/silixa_v8.1/
--rw-r--r--   0 runner    (1001) docker     (121)   286652 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.498999 dtscalibration-1.1.2/tests/data/single_ended/
--rwxr-xr-x   0 runner    (1001) docker     (121)    88932 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132202074.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)    88936 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132232903.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)    88888 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132303723.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:03:34.502999 dtscalibration-1.1.2/tests/data/zipped data/
--rw-r--r--   0 runner    (1001) docker     (121)   166974 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/zipped data/double_ended.zip
--rw-r--r--   0 runner    (1001) docker     (121)   255063 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/zipped data/double_ended2.zip
--rw-r--r--   0 runner    (1001) docker     (121)  1508174 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/zipped data/double_single_ended.zip
--rw-r--r--   0 runner    (1001) docker     (121)   260862 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/zipped data/silixa_v4.5.zip
--rw-r--r--   0 runner    (1001) docker     (121)    78779 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/data/zipped data/single_ended.zip
--rw-r--r--   0 runner    (1001) docker     (121)    19464 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (121)   117032 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/test_dtscalibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-09-25 16:03:24.000000 dtscalibration-1.1.2/tox.ini
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.coveragerc
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.editorconfig
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.style.yapf
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.zenodo.json
+-rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CITATION.cff
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/_config.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/index.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/installation.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/learn_by_examples.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/nb_examples_to_docs.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/readme.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/usage.rst
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.DataStore.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.check_dims.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.check_timestep_allclose.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.get_netcdf_encoding.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.merge_double_ended.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.open_datastore.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.open_mf_datastore.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_accuracy.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_location_residuals_double_ended.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_residuals_reference_sections.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_residuals_reference_sections_single.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_sigma_report.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_apsensing_files.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_sensornet_files.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_sensortran_files.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_silixa_files.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.shift_double_ended.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.suggest_cable_shift_double_ended.rst
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/01Load_xml_measurement_files.ipynb
+-rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/03Define_sections.ipynb
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/04Calculate_variance_Stokes.ipynb
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/05Calibrate_single_ols.ipynb
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/06Calibrate_double_ols.ipynb
+-rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/07Calibrate_single_wls.ipynb
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/08Calibrate_double_wls.ipynb
+-rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/09Import_timeseries.ipynb
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/10Align_double_ended_measurements.ipynb
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/13Fixed_parameter_calibration.ipynb
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/14Lossy_splices.ipynb
+-rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/15Matching_sections.ipynb
+-rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/16Averaging_temperatures.ipynb
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A2Load_sensornet_files.ipynb
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A3Load_ap_sensing_files.ipynb
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A4Load_sensortran_files.ipynb
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/reference/index.rst
+-rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/Added uncertainty from fixing parameters.pdf
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/README.md
+-rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/temperature_variance_from_stokes.pdf
+-rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
+-rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/__init__.py
+-rw-r--r--   0        0        0    51325 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/calibrate_utils.py
+-rw-r--r--   0        0        0   241203 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/datastore.py
+-rw-r--r--   0        0        0    12525 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/datastore_utils.py
+-rw-r--r--   0        0        0    60445 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/io.py
+-rwxr-xr-x   0        0        0    24378 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_datastore.py
+-rw-r--r--   0        0        0   116952 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_dtscalibration.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_examples.py
+-rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
+-rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
+-rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
+-rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112245510.xml
+-rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112746818.xml
+-rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921113248085.xml
+-rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014052498.xml
+-rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014057119.xml
+-rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014101652.xml
+-rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014106243.xml
+-rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014110917.xml
+-rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014115480.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/info.txt
+-rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
+-rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
+-rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
+-rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
+-rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
+-rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
+-rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
+-rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
+-rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
+-rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
+-rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
+-rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
+-rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
+-rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
+-rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
+-rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
+-rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
+-rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
+-rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
+-rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
+-rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
+-rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
+-rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
+-rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
+-rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
+-rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
+-rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
+-rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
+-rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
+-rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
+-rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
+-rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
+-rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
+-rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
+-rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
+-rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
+-rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
+-rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
+-rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
+-rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
+-rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
+-rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
+-rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
+-rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
+-rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
+-rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132202074.xml
+-rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132232903.xml
+-rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132303723.xml
+-rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_ended.zip
+-rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_ended2.zip
+-rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_single_ended.zip
+-rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/silixa_v4.5.zip
+-rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/single_ended.zip
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.gitignore
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/README.rst
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/PKG-INFO
```

### Comparing `dtscalibration-1.1.2/.style.yapf` & `dtscalibration-1.2.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/.zenodo.json` & `dtscalibration-1.2.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/CHANGELOG.rst` & `dtscalibration-1.2.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 
 Changelog
 =========
+[1.2.0] (13-03-2023)
+
+Bugfixes
+
+* Fixed deprecated np.float and np.int
+
+Other
+
+* Moved project build system & scripts to hatch.
+* Project is now fully configured using pyproject.toml
+* Linting is handled by Ruff.
+* Notebooks are now rendered as part of the documentation.
+
+Removed
+
+* cli.py script (unused) has been removed.
+
+New contributors:
+* Karl Lapo (@klapo)
+
 1.1.2 (2022-09-25)
 ------------------
 
 * Added support for Sensornet Sentinel v5 files.
 
 
 1.1.1 (2022-09-25)
```

### Comparing `dtscalibration-1.1.2/CITATION.cff` & `dtscalibration-1.2.0/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
   - calibration
   - Python
 cff-version: "1.0.3"
 doi: "10.5281/zenodo.1410097"
 license: "BSD-3-Clause"
 repository-code: "https://github.com/dtscalibration/python-dts-calibration"
 title: "Python distributed temperature sensing calibration"
-version: "v1.1.2"
+version: "v1.2.0"
 url: "https://python-dts-calibration.readthedocs.io"
```

### Comparing `dtscalibration-1.1.2/CONTRIBUTING.rst` & `dtscalibration-1.2.0/CONTRIBUTING.rst`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
 Bug reports
 ===========
 
-When `reporting a bug <https://github.com/bdestombe/python-dts-calibration/issues>`_ please include:
+When `reporting a bug <https://github.com/dtscalibration/python-dts-calibration/issues>`_ please include:
 
     * Your operating system name and version.
     * Any details about your local setup that might be helpful in troubleshooting.
     * Detailed steps to reproduce the bug.
 
 Documentation improvements
 ==========================
@@ -20,42 +20,48 @@
 dtscalibration could always use more documentation, whether as part of the
 official dtscalibration docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Feature requests and feedback
 =============================
 
-The best way to send feedback is to file an issue at https://github.com/bdestombe/python-dts-calibration/issues.
+The best way to send feedback is to file an issue at https://github.com/dtscalibration/python-dts-calibration/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that code contributions are welcome :)
 
 Development
 ===========
 
 To set up `python-dts-calibration` for local development:
 
-1. Fork `python-dts-calibration <https://github.com/bdestombe/python-dts-calibration>`_
+1. Fork `python-dts-calibration <https://github.com/dtscalibration/python-dts-calibration>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
     git clone git@github.com:your_name_here/python-dts-calibration.git
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes, run all the checks, doc builder and spell checker with `tox <http://tox.readthedocs.io/en/latest/install.html>`_ one command::
+4. Activate your desired development environment (e.g., a python venv or conda environment), and install the package in editable mode, with the dev dependencies::
 
-    tox
+    pip install -e .[dev]
+
+4. When you're done making changes, make sure the code follows the right style, that all tests pass, and that the docs build with the following commands::
+
+    hatch run format
+    hatch run test
+    hatch run docs:build
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
     git push origin name-of-your-bugfix-or-feature
 
@@ -64,27 +70,23 @@
 Pull Request Guidelines
 -----------------------
 
 If you need some code review or feedback while you're developing the code just make the pull request.
 
 For merging, you should:
 
-1. Include passing tests (run ``tox``) [1]_.
+1. Include passing tests (do ``hatch run test``) [1]_.
 2. Update documentation when there's new API, functionality etc.
 3. Add a note to ``CHANGELOG.rst`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/bdestombe/python-dts-calibration/pull_requests>`_ for each change you add in the pull request.
-
-       It will be slower though ...
+.. [1] Sometimes there are issues with different python versions. For this you can do
+       ``hatch run test_matrix:test``. Generally, on Github tests will be run using Github Actions,
+       where all versions, as well as the documentation, are tested.
+       This will be slower though ...
 
 Tips
 ----
 
 To run a subset of tests::
 
-    tox -e envname -- pytest -k test_myfeature
-
-To run all the test environments in *parallel* (you need to ``pip install detox``)::
-
-    detox
+    hatch run pytest -k test_myfeature
```

### Comparing `dtscalibration-1.1.2/LICENSE` & `dtscalibration-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/MANIFEST.in` & `dtscalibration-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/README.rst` & `dtscalibration-1.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,30 +10,28 @@
       - |docs|
     * - Tests
       - |tests|
     * - Package
       - | |version| |supported-versions| |commits-since|
     * - Citable
       - |zenodo|
-    * - Example notebooks
-      - |example-notebooks|
 
 .. |docs| image:: https://readthedocs.org/projects/python-dts-calibration/badge/?style=flat
     :target: https://python-dts-calibration.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. |tests| image:: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml/badge.svg
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v1.1.2.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v1.2.0.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -41,18 +39,14 @@
     :alt: Supported versions
     :target: https://pypi.python.org/pypi/dtscalibration
 
 .. |zenodo| image:: https://zenodo.org/badge/143077491.svg
    :alt: It would be greatly appreciated if you could cite this package in eg articles presentations
    :target: https://zenodo.org/badge/latestdoi/143077491
 
-.. |example-notebooks| image:: https://mybinder.org/badge.svg
-   :alt: Interactively run the example notebooks online
-   :target: https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?filepath=examples%2Fnotebooks
-
 .. end-badges
 
 A Python package to load Distributed Temperature Sensing files, perform a calibration, and plot the result. A detailed description of the calibration procedure can be found at https://doi.org/10.3390/s20082235 .
 
 * Free software: BSD 3-Clause License
 
 
@@ -86,22 +80,20 @@
 Devices currently supported
 ===========================
 * Silixa Ltd.: **Ultima** & **XT-DTS** .xml files *(up to version 8.1)*
 * Sensornet Ltd.: **Oryx**, **Halo** & **Sentinel** .ddf files
 * AP Sensing: **CP320** .xml files *(single ended only)*
 * SensorTran: **SensorTran 5100** .dat binary files *(single ended only)*
 
-Learn by examples
-=================
-Interactively run the example notebooks online by clicking `here <https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?filepath=examples%2Fnotebooks>`_.
-
 Documentation
 =============
 
 https://python-dts-calibration.readthedocs.io/
+Example notebooks can be viewed [here](https://python-dts-calibration.readthedocs.io/en/latest/learn_by_examples.html).
+
 
 How to cite
 ===========
 The following article explains and discusses the calibration procedure:
 
     des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235
```

### Comparing `dtscalibration-1.1.2/docs/api/dtscalibration.DataStore.rst` & `dtscalibration-1.2.0/docs/api/dtscalibration.DataStore.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/docs/conf.py` & `dtscalibration-1.2.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'sphinx.ext.doctest',
     'sphinx.ext.extlinks',
     'sphinx.ext.ifconfig',
     'sphinx.ext.napoleon',
     'sphinx.ext.todo',
     'sphinx.ext.viewcode',
     'sphinx.ext.autosectionlabel',
-    # 'nbsphinx',
+    'nbsphinx',
     'sphinx.ext.mathjax',
     'sphinx.ext.intersphinx',
     'sphinx_automodapi.automodapi',
     'sphinx_automodapi.smart_resolver',
     'IPython.sphinxext.ipython_directive',
     'IPython.sphinxext.ipython_console_highlighting',
     # 'matplotlib.sphinxext.mathmpl',
@@ -26,26 +26,26 @@
     # >3.0.0
     'matplotlib.sphinxext.plot_directive',
     # 'matplotlib.sphinxext.ipython_directive',
     'recommonmark',  # Parses markdown
     ]
 
 if os.getenv('SPELLCHECK'):
-    extensions += 'sphinxcontrib.spelling',
+    extensions += 'sphinxcontrib.spelling'
     spelling_show_suggestions = True
     spelling_lang = 'en_US'
 
 
 source_suffix = ['.rst', '.md']
 master_doc = 'index'
 project = 'dtscalibration'
 year = str(date.today().year)
 author = 'Bas des Tombe and Bart Schilperoort'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '1.1.2'
+version = release = '1.2.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/dtscalibration/python-dts-calibration/issues'
               '/%s', '#'),
     'pr': ('https://github.com/dtscalibration/python-dts-calibration/pull/%s',
@@ -65,7 +65,11 @@
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
 
 # sphinx_automodapi.automodapi
 numpydoc_show_class_members = False
+
+# -- nbsphinx configuration --
+nbsphinx_allow_errors = False
+nbsphinx_execute = "always"
```

### Comparing `dtscalibration-1.1.2/docs/examples/index.rst` & `dtscalibration-1.2.0/docs/learn_by_examples.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Learn by Examples
 =================
 
 .. toctree::
-    notebooks/01Load_xml_measurement_files.ipynb.rst
-    notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb.rst
-    notebooks/03Define_sections.ipynb.rst
-    notebooks/04Calculate_variance_Stokes.ipynb.rst
-    notebooks/05Calibrate_single_ols.ipynb.rst
-    notebooks/06Calibrate_double_ols.ipynb.rst
-    notebooks/07Calibrate_single_wls.ipynb.rst
-    notebooks/08Calibrate_double_wls.ipynb.rst
-    notebooks/09Import_timeseries.ipynb.rst
-    notebooks/10Align_double_ended_measurements.ipynb.rst
-    notebooks/11Merge_single_measurements_into_double.ipynb.rst
-    notebooks/12Datastore_from_numpy_arrays.ipynb.rst
-    notebooks/13Fixed_parameter_calibration.ipynb.rst
-    notebooks/14Lossy_splices.ipynb.rst
-    notebooks/15Matching_sections.ipynb.rst
-    notebooks/16Averaging_temperatures.ipynb.rst
-    notebooks/A2Load_sensornet_files.ipynb.rst
-    notebooks/A3Load_ap_sensing_files.ipynb.rst
-    notebooks/A4Load_sensortran_files.ipynb.rst
+    notebooks/01Load_xml_measurement_files.ipynb
+    notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb
+    notebooks/03Define_sections.ipynb
+    notebooks/04Calculate_variance_Stokes.ipynb
+    notebooks/05Calibrate_single_ols.ipynb
+    notebooks/06Calibrate_double_ols.ipynb
+    notebooks/07Calibrate_single_wls.ipynb
+    notebooks/08Calibrate_double_wls.ipynb
+    notebooks/09Import_timeseries.ipynb
+    notebooks/10Align_double_ended_measurements.ipynb
+    notebooks/11Merge_single_measurements_into_double.ipynb
+    notebooks/12Datastore_from_numpy_arrays.ipynb
+    notebooks/13Fixed_parameter_calibration.ipynb
+    notebooks/14Lossy_splices.ipynb
+    notebooks/15Matching_sections.ipynb
+    notebooks/16Averaging_temperatures.ipynb
+    notebooks/A2Load_sensornet_files.ipynb
+    notebooks/A3Load_ap_sensing_files.ipynb
+    notebooks/A4Load_sensortran_files.ipynb
```

### Comparing `dtscalibration-1.1.2/docs/nb_examples_to_docs.py` & `dtscalibration-1.2.0/docs/nb_examples_to_docs.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/src/dtscalibration/__init__.py` & `dtscalibration-1.2.0/src/dtscalibration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .datastore_utils import suggest_cable_shift_double_ended
 from .plot import plot_accuracy
 from .plot import plot_location_residuals_double_ended
 from .plot import plot_residuals_reference_sections
 from .plot import plot_residuals_reference_sections_single
 from .plot import plot_sigma_report
 
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 __all__ = [
     "DataStore", "open_datastore", "open_mf_datastore", "read_apsensing_files",
     "read_sensornet_files", "read_sensortran_files", "read_silixa_files",
     'check_dims', 'check_timestep_allclose', 'get_netcdf_encoding',
     'merge_double_ended', 'shift_double_ended',
     'suggest_cable_shift_double_ended', 'plot_accuracy',
     'plot_location_residuals_double_ended',
```

### Comparing `dtscalibration-1.1.2/src/dtscalibration/calibrate_utils.py` & `dtscalibration-1.2.0/src/dtscalibration/calibrate_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/src/dtscalibration/datastore.py` & `dtscalibration-1.2.0/src/dtscalibration/datastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -2100,15 +2100,15 @@
                                 split['X_gamma'], split['X_dalpha'],
                                 split['X_c'], split['X_TA'])),
                         split['X_m'])).tocsr()
                 p_val = split['p0_est_dalpha'].copy()
                 ip_use = list(range(1 + 1 + nt + nta * nt))
 
             p_var = np.zeros_like(p_val)
-            p_cov = np.zeros((p_val.size, p_val.size), dtype=np.float)
+            p_cov = np.zeros((p_val.size, p_val.size), dtype=float)
 
             if fix_gamma is not None:
                 ip_remove = [0]
                 ip_use = [i for i in ip_use if i not in ip_remove]
                 p_val[ip_remove] = fix_gamma[0]
                 p_var[ip_remove] = fix_gamma[1]
 
@@ -4421,16 +4421,16 @@
 
         Four types of averaging are implemented. Please see Example Notebook 16.
 
         Parameters
         ----------
         p_val : array-like, optional
             Define `p_val`, `p_var`, `p_cov` if you used an external function
-            for calibration. Has size 2 + `nt`. First value is :math:`\gamma`,
-            second is :math:`\Delta \\alpha`, others are :math:`C` for each
+            for calibration. Has size 2 + `nt`. First value is :math:`\\gamma`,
+            second is :math:`\\Delta \\alpha`, others are :math:`C` for each
             timestep.
             If set to False, no uncertainty in the parameters is propagated
             into the confidence intervals. Similar to the spec sheets of the DTS
             manufacturers. And similar to passing an array filled with zeros
         p_cov : array-like, optional
             The covariances of `p_val`.
         st_var, ast_var, rst_var, rast_var : float, callable, array-like, optional
```

### Comparing `dtscalibration-1.1.2/src/dtscalibration/datastore_utils.py` & `dtscalibration-1.2.0/src/dtscalibration/datastore_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/src/dtscalibration/io.py` & `dtscalibration-1.2.0/src/dtscalibration/io.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/src/dtscalibration/plot.py` & `dtscalibration-1.2.0/src/dtscalibration/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,16 +309,16 @@
         right=0.9,
         top=0.88)
     main_ax = fig.add_subplot(grid[2:, 2:-1])
     y_ax_avg = fig.add_subplot(grid[2:, :2])  # xticklabels=[],
     x_ax_avg = fig.add_subplot(grid[:2, 2:-1])  # , sharex=main_ax
     legend_ax = fig.add_subplot(grid[:2, :2], xticklabels=[], yticklabels=[])
     cbar_ax = fig.add_subplot(grid[2:, -1], xticklabels=[], yticklabels=[])
-    if np.issubdtype(resid[time_dim].dtype, np.float) or np.issubdtype(
-            resid[time_dim].dtype, np.int):
+    if np.issubdtype(resid[time_dim].dtype, float) or np.issubdtype(
+            resid[time_dim].dtype, int):
         resid.plot.imshow(
             ax=main_ax,
             cbar_ax=cbar_ax,
             cbar_kwargs={"aspect": 10},
             robust=robust)
     else:
         resid.plot(
```

### Comparing `dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml` & `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml` & `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml` & `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921112245510.xml` & `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112245510.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921112746818.xml` & `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112746818.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended/channel 1_20170921113248085.xml` & `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921113248085.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014052498.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014052498.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014057119.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014057119.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014101652.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014101652.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014106243.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014106243.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014110917.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014110917.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_ended2/channel 1_20180328014115480.xml` & `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014115480.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml` & `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv` & `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv` & `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv` & `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf` & `dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat` & `dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml` & `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml` & `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml` & `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml` & `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml` & `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml` & `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml` & `dtscalibration-1.2.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132202074.xml` & `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132202074.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132232903.xml` & `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132232903.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/single_ended/channel 2_20180504132303723.xml` & `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132303723.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/zipped data/double_ended.zip` & `dtscalibration-1.2.0/tests/data/zipped data/double_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/zipped data/double_ended2.zip` & `dtscalibration-1.2.0/tests/data/zipped data/double_ended2.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/zipped data/double_single_ended.zip` & `dtscalibration-1.2.0/tests/data/zipped data/double_single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/zipped data/silixa_v4.5.zip` & `dtscalibration-1.2.0/tests/data/zipped data/silixa_v4.5.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/data/zipped data/single_ended.zip` & `dtscalibration-1.2.0/tests/data/zipped data/single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/test_datastore.py` & `dtscalibration-1.2.0/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.1.2/tests/test_dtscalibration.py` & `dtscalibration-1.2.0/tests/test_dtscalibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import scipy.sparse as sp
 from scipy import stats
 
 from dtscalibration import DataStore
 from dtscalibration import read_silixa_files
 from dtscalibration.calibrate_utils import wls_sparse
 from dtscalibration.calibrate_utils import wls_stats
-from dtscalibration.cli import main
 
 np.random.seed(0)
 
 fn = [
     "channel 1_20170921112245510.xml", "channel 1_20170921112746818.xml",
     "channel 1_20170921112746818.xml"]
 fn_single = [
@@ -52,18 +51,14 @@
         print(m)
 
     desired2 = np.broadcast_to(desired, actual.shape)
     np.testing.assert_almost_equal(actual, desired2, err_msg=m, **kwargs)
     pass
 
 
-def test_main():
-    assert main([]) == 0
-
-
 def test_variance_input_types_single():
     import dask.array as da
 
     from src.dtscalibration import DataStore
 
     state = da.random.RandomState(0)
```

### Comparing `dtscalibration-1.1.2/tests/test_examples.py` & `dtscalibration-1.2.0/tests/test_examples.py`

 * *Files identical despite different names*


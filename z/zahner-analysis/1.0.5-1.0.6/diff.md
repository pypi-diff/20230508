# Comparing `tmp/zahner_analysis-1.0.5.tar.gz` & `tmp/zahner_analysis-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zahner_analysis-1.0.5.tar", last modified: Thu May  4 14:05:06 2023, max compression
+gzip compressed data, was "zahner_analysis-1.0.6.tar", last modified: Mon May  8 06:33:41 2023, max compression
```

## Comparing `zahner_analysis-1.0.5.tar` & `zahner_analysis-1.0.6.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.175227 zahner_analysis-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/BasicIntroduction/
--rw-r--r--   0 runner    (1001) docker     (123)   459849 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/AnalysisScreenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)   152479 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/
--rw-r--r--   0 runner    (1001) docker     (123)   105801 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.png
--rw-r--r--   0 runner    (1001) docker     (123)   100508 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.svg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted_simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-data.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)   374829 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/
--rw-r--r--   0 runner    (1001) docker     (123)    89466 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132610 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png
--rw-r--r--   0 runner    (1001) docker     (123)    79494 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)    45584 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-battery.ism
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/
--rw-r--r--   0 runner    (1001) docker     (123)    61065 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py
--rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/Examples/ZHIT/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/RC-R-L.isfx
--rw-r--r--   0 runner    (1001) docker     (123)   434541 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/drift.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/jupyter
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/matplotlib
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/numpy
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/requests
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/scipy
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/analysis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29914 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/eis_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/zahner_analysis/file_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/impedance_model_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/isc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/ism_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/iss_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/seqtxt_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/thales_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/zahner_analysis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/plotting/impedance_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.810982 zahner_analysis-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.786982 zahner_analysis-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.790982 zahner_analysis-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.786982 zahner_analysis-1.0.6/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.790982 zahner_analysis-1.0.6/Examples/BasicIntroduction/
+-rw-r--r--   0 runner    (1001) docker     (123)   459849 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/AnalysisScreenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   152479 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/BasicIntroduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/BasicIntroduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.790982 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/
+-rw-r--r--   0 runner    (1001) docker     (123)   105801 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/bode.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100508 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/rc-data.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/BasicIntroduction/rc-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.790982 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)   374829 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.794982 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    89466 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132610 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79494 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)    45584 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/li-ion-battery.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/li-ion-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.794982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    61065 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.786982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.794982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.794982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.794982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.798982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.802982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.802982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.802982 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/Examples/ZHIT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ZHIT/RC-R-L.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)   434541 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/Examples/ZHIT/drift.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSES/jupyter
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSES/matplotlib
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSES/numpy
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSES/requests
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/LICENSES/scipy
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-08 06:33:41.810982 zahner_analysis-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:33:41.810982 zahner_analysis-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/zahner_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/zahner_analysis/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/analysis_tools/analysis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29914 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/analysis_tools/eis_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/analysis_tools/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/zahner_analysis/file_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/impedance_model_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/isc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/ism_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/iss_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/seqtxt_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/file_import/thales_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/zahner_analysis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-05-08 06:33:32.000000 zahner_analysis-1.0.6/zahner_analysis/plotting/impedance_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:33:41.806982 zahner_analysis-1.0.6/zahner_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-08 06:33:41.000000 zahner_analysis-1.0.6/zahner_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-08 06:33:41.000000 zahner_analysis-1.0.6/zahner_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:33:41.000000 zahner_analysis-1.0.6/zahner_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 06:33:41.000000 zahner_analysis-1.0.6/zahner_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 06:33:41.000000 zahner_analysis-1.0.6/zahner_analysis.egg-info/top_level.txt
```

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/AnalysisScreenshot.png` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/AnalysisScreenshot.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.ipynb` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/BasicIntroduction.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.py` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/BasicIntroduction.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.png` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/bode.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.svg` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/bode.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_result.json` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted.isfx` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/simulated.ism` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/fit_results/simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-data.ism` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/rc-data.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-model.isfx` & `zahner_analysis-1.0.6/Examples/BasicIntroduction/rc-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode.svg` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_result.json` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-battery.ism` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/li-ion-battery.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-model.isfx` & `zahner_analysis-1.0.6/Examples/ComplexFitConfigurations/li-ion-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism` & `zahner_analysis-1.0.6/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ZHIT/RC-R-L.isfx` & `zahner_analysis-1.0.6/Examples/ZHIT/RC-R-L.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ipynb` & `zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ism` & `zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.py` & `zahner_analysis-1.0.6/Examples/ZHIT/ZHIT.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/Examples/ZHIT/drift.ism` & `zahner_analysis-1.0.6/Examples/ZHIT/drift.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSE` & `zahner_analysis-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSES/jupyter` & `zahner_analysis-1.0.6/LICENSES/jupyter`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSES/matplotlib` & `zahner_analysis-1.0.6/LICENSES/matplotlib`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSES/numpy` & `zahner_analysis-1.0.6/LICENSES/numpy`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSES/requests` & `zahner_analysis-1.0.6/LICENSES/requests`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/LICENSES/scipy` & `zahner_analysis-1.0.6/LICENSES/scipy`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/PKG-INFO` & `zahner_analysis-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zahner_analysis
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for the analysis of electrochemical impedance spectra.
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
         Copyright (c) 2022 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zahner_analysis-1.0.5/README.md` & `zahner_analysis-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/openapi.yaml` & `zahner_analysis-1.0.6/openapi.yaml`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/pyproject.toml` & `zahner_analysis-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/analysis_connection.py` & `zahner_analysis-1.0.6/zahner_analysis/analysis_tools/analysis_connection.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/eis_fitting.py` & `zahner_analysis-1.0.6/zahner_analysis/analysis_tools/eis_fitting.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/error.py` & `zahner_analysis-1.0.6/zahner_analysis/analysis_tools/error.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/impedance_model_import.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/impedance_model_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/isc_import.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/isc_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/ism_import.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/ism_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,27 +23,28 @@
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
 THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import numpy as np
 import datetime
 import io
 import os
+import datetime
 from typing import Union
 
 from zahner_analysis.file_import.thales_file_utils import *
 
 
 class IsmImport:
-    """Class to be able to read ism files (EIS data).
+    """
+    Class to be able to read ism files (EIS data).
 
     This class extracts the data from the ism files.
     It returns the data for the frequency range between the reversal frequency and the end frequency.
 
     :param file: The path to the ism file, or the ism file as bytes or bytearray.
-    :type file: str, bytes, bytearray
     """
 
     def __init__(self, filename: Union[str, bytes, bytearray]):
         self._filename = "FromBytes.ism"
         if isinstance(filename, bytes) or isinstance(filename, bytearray):
             self._binaryFileContent = filename
             ismFile = io.BytesIO(filename)
@@ -117,150 +118,167 @@
             self.swapNecessary = True
             self.fromIndex = self.maxFrequencyIndex
             self.toIndex = self.minFrequencyIndex
 
         self.toIndex += 1
         return
 
-    def getNumberOfSamples(self):
-        """Returns the complete number of samples.
+    def getNumberOfSamples(self) -> int:
+        """
+        Returns the complete number of samples.
 
         This function returns the number of samples in the ism file.
-        This number can be greater than the number of elements returned in the arrays.
-        For the arrays, only the largest frequency range from minimum to maximum frequency is returned,
-        not the overlapping range.
 
         :returns: Number of total samples.
         """
         return self.numberOfSamples
 
-    def getFrequencyArray(self):
-        """Get the frequency points from the measurement.
+    def _arraySlice(
+        self, array: np.ndarray, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
+        """
+        Can return the array range without duplicate frequency support points.
 
-        The frequency points between the reversal frequency and the final frequency are returned.
+        For numpy and other libraries there must not be any duplicate frequency support points, therefore this function trims the array range.
 
-        :returns: Numpy array with the frequency points.
+        :param array: Array that is processed.
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
+        :return: The eventually trimmed array.
         """
+        retval = array
+        if includeDoubleFrequencies is False:
+            retval = retval[self.fromIndex : self.toIndex]
+
         if self.swapNecessary:
-            return np.flip(self.frequency[self.fromIndex : self.toIndex])
+            return np.flip(retval)
         else:
-            return self.frequency[self.fromIndex : self.toIndex]
+            return retval
 
-    def getImpedanceArray(self):
-        """Get the impedance points from the measurement.
+    def getFrequencyArray(self, includeDoubleFrequencies: bool = False) -> np.ndarray:
+        """
+        Get the frequency points from the measurement.
 
-        The impedance points between the reversal frequency and the final frequency are returned.
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
+        :returns: Numpy array with the frequency points.
+        """
+        return self._arraySlice(self.frequency, includeDoubleFrequencies)
 
-        :returns: Numpy array with the impedance points.
+    def getImpedanceArray(self, includeDoubleFrequencies: bool = False) -> np.ndarray:
         """
-        if self.swapNecessary:
-            return np.flip(self.impedance[self.fromIndex : self.toIndex])
-        else:
-            return self.impedance[self.fromIndex : self.toIndex]
+        Get the impedance points from the measurement.
 
-    def getPhaseArray(self, degree=False):
-        """Get the phase points from the measurement.
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
+        :returns: Numpy array with the impedance points.
+        """
+        return self._arraySlice(self.impedance, includeDoubleFrequencies)
 
-        The phase points between the reversal frequency and the final frequency are returned.
+    def getPhaseArray(
+        self, degree: bool = False, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
+        """
+        Get the phase points from the measurement.
 
+        :param degree: True for phase in degree, default radiant.
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
         :returns: Numpy array with the phase points as radiant.
         """
         radToDegree = 1.0
         if degree == True:
             radToDegree = 360 / (2 * np.pi)
-        if self.swapNecessary:
-            return np.flip(self.phase[self.fromIndex : self.toIndex] * radToDegree)
-        else:
-            return self.phase[self.fromIndex : self.toIndex] * radToDegree
 
-    def getComplexImpedanceArray(self):
-        """Get the complex impedance points from the measurement.
+        return self._arraySlice(self.phase, includeDoubleFrequencies) * radToDegree
 
-        The complex impedance points between the reversal frequency and the final frequency are returned.
+    def getComplexImpedanceArray(
+        self, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
+        """
+        Get the complex impedance points from the measurement.
 
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
         :returns: Numpy array with the complex impedance points.
         """
-        imp = self.getImpedanceArray()
-        phase = self.getPhaseArray()
-
+        imp = self.getImpedanceArray(includeDoubleFrequencies)
+        phase = self.getPhaseArray(includeDoubleFrequencies=includeDoubleFrequencies)
         return np.cos(phase) * imp + 1j * np.sin(phase) * imp
 
-    def getSignificanceArray(self):
-        """Get the significance points from the measurement.
-
-        The significance points between the reversal frequency and the final frequency are returned.
+    def getSignificanceArray(
+        self, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
+        """
+        Get the significance points from the measurement.
 
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
         :returns: Numpy array with the significance points.
         """
-        if self.swapNecessary:
-            return np.flip(self.significance[self.fromIndex : self.toIndex])
-        else:
-            return self.significance[self.fromIndex : self.toIndex]
+        return self._arraySlice(self.significance, includeDoubleFrequencies)
 
-    def getMeasurementDateTimeArray(self):
-        """Get the timestamps from the measurement.
-
-        The timestamps between the reversal frequency and the final frequency are returned.
-        The smallest time is the reversal point. The start time is not included in this array because
-        the overlapping points are not returned.
+    def getMeasurementDateTimeArray(
+        self, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
+        """
+        Get the timestamps from the measurement.
 
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
         :returns: Numpy array with the datetime objects.
         """
-        if self.swapNecessary:
-            return np.flip(self.measurementTimeStamp[self.fromIndex : self.toIndex])
-        else:
-            return self.measurementTimeStamp[self.fromIndex : self.toIndex]
+        return self._arraySlice(self.measurementTimeStamp, includeDoubleFrequencies)
 
-    def getMeasurementStartDateTime(self):
-        """Get the start date time of the measurement.
+    def getMeasurementStartDateTime(self) -> datetime.datetime:
+        """
+        Get the start date time of the measurement.
 
         Returns the start datetime of the measurement.
 
         :returns: datetime object with the start time of the measurement.
         """
         return min(self.measurementTimeStamp)
 
-    def getMeasurementEndDateTime(self):
-        """Get the end date time of the measurement.
+    def getMeasurementEndDateTime(self) -> datetime.datetime:
+        """
+        Get the end date time of the measurement.
 
         Returns the end datetime of the measurement.
 
         :returns: datetime object with the end time of the measurement.
         """
         return max(self.measurementTimeStamp)
 
     def save(self, filename):
-        """Save the impedance data.
+        """
+        Save the impedance data.
 
         Only the binary file content that has been read is saved. If the data is edited, this is not saved.
 
         :param filename: Path and filename of the file to be saved with the extension .ism.
         """
         with open(filename, "wb") as f:
             f.write(self._binaryFileContent)
         return
 
-    def getFileName(self):
-        """Get the name of the file.
+    def getFileName(self) -> str:
+        """
+        Get the name of the file.
 
         :returns: The filename if the file was opened or "FromBytes.ism" if it was created from bytearrays.
         """
         return self._filename
 
-    def getBinaryFileContent(self):
-        """Get the content of the file binary.
+    def getBinaryFileContent(self) -> bytearray:
+        """
+        Get the content of the file binary.
 
         Returns the file contents as a binary byte array.
 
         :returns: bytearray with the file content.
         """
         return self._binaryFileContent
 
-    def getMetaData(self):
-        """Get the meta data of the file binary.
+    def getMetaData(self) -> bytearray:
+        """
+        Get the meta data of the file binary.
 
         Returns the file contents as a binary byte array.
 
         :returns: bytearray with the file content.
         """
         return self._metaData
 
@@ -268,15 +286,18 @@
         """
         returns a list with the different data tracks.
 
         :returns: List with the track names.
         """
         return list(map(str, self.acqChannels.keys()))
 
-    def getTrack(self, track: str) -> np.ndarray:
+    def getTrack(
+        self, track: str, includeDoubleFrequencies: bool = False
+    ) -> np.ndarray:
         """
         returns an array with the points for the given track.
 
-        :param track: name of the track
+        :param track: name of the track.
+        :param includeDoubleFrequencies: If True, all measurement data are returned, if False, only the largest non-overlapping area is returned. Defaults to False.
         :returns: Numpy array with the track.
         """
-        return self.acqChannels[track]
+        return self._arraySlice(self.acqChannels[track], includeDoubleFrequencies)
```

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/iss_import.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/iss_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/seqtxt_import.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/seqtxt_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/file_import/thales_file_utils.py` & `zahner_analysis-1.0.6/zahner_analysis/file_import/thales_file_utils.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis/plotting/impedance_plot.py` & `zahner_analysis-1.0.6/zahner_analysis/plotting/impedance_plot.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.5/zahner_analysis.egg-info/PKG-INFO` & `zahner_analysis-1.0.6/zahner_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zahner-analysis
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for the analysis of electrochemical impedance spectra.
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
         Copyright (c) 2022 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zahner_analysis-1.0.5/zahner_analysis.egg-info/SOURCES.txt` & `zahner_analysis-1.0.6/zahner_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/EnergyCapSdk-8.2302.4520.tar.gz` & `tmp/EnergyCapSdk-8.2302.4532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnergyCapSdk-8.2302.4520.tar", last modified: Wed Apr 26 10:27:47 2023, max compression
+gzip compressed data, was "EnergyCapSdk-8.2302.4532.tar", last modified: Mon May  8 15:07:49 2023, max compression
```

## Comparing `EnergyCapSdk-8.2302.4520.tar` & `EnergyCapSdk-8.2302.4532.tar`

### file list

```diff
@@ -1,1900 +1,1900 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:27:47.573401 EnergyCapSdk-8.2302.4520/
-drwxrwxrwx   0        0        0        0 2023-04-26 10:27:24.507729 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/
--rw-rw-rw-   0        0        0      293 2023-04-26 10:27:23.000000 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0   101423 2023-04-26 10:27:23.000000 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:27:23.000000 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 10:27:23.000000 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 10:27:23.000000 EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      293 2023-04-26 10:27:47.572223 EnergyCapSdk-8.2302.4520/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 10:27:24.517501 EnergyCapSdk-8.2302.4520/energycap/
--rw-rw-rw-   0        0        0       56 2023-04-26 10:27:14.000000 EnergyCapSdk-8.2302.4520/energycap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:27:24.688155 EnergyCapSdk-8.2302.4520/energycap/sdk/
--rw-rw-rw-   0        0        0      437 2023-04-26 10:27:14.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/__init__.py
--rw-rw-rw-   0        0        0  1640151 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/energy_cap_api.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:27:47.567839 EnergyCapSdk-8.2302.4520/energycap/sdk/models/
--rw-rw-rw-   0        0        0   165177 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request.py
--rw-rw-rw-   0        0        0     2181 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request_py3.py
--rw-rw-rw-   0        0        0     2321 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response.py
--rw-rw-rw-   0        0        0     2356 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response_py3.py
--rw-rw-rw-   0        0        0     2174 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request.py
--rw-rw-rw-   0        0        0     2194 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request_py3.py
--rw-rw-rw-   0        0        0     2334 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response.py
--rw-rw-rw-   0        0        0     2369 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response_py3.py
--rw-rw-rw-   0        0        0     2157 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request.py
--rw-rw-rw-   0        0        0     2177 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request_py3.py
--rw-rw-rw-   0        0        0     2317 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response.py
--rw-rw-rw-   0        0        0     2352 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response_py3.py
--rw-rw-rw-   0        0        0     1964 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_request.py
--rw-rw-rw-   0        0        0     1960 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_request_py3.py
--rw-rw-rw-   0        0        0     1426 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_response.py
--rw-rw-rw-   0        0        0     1442 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_response_py3.py
--rw-rw-rw-   0        0        0     1245 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_audit_enable.py
--rw-rw-rw-   0        0        0     1260 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_audit_enable_py3.py
--rw-rw-rw-   0        0        0     2068 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child.py
--rw-rw-rw-   0        0        0     2123 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_py3.py
--rw-rw-rw-   0        0        0     2317 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_with_type.py
--rw-rw-rw-   0        0        0     2371 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_with_type_py3.py
--rw-rw-rw-   0        0        0     1038 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_child.py
--rw-rw-rw-   0        0        0     1057 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_child_py3.py
--rw-rw-rw-   0        0        0     1913 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_request.py
--rw-rw-rw-   0        0        0     1938 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_request_py3.py
--rw-rw-rw-   0        0        0     1634 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_response.py
--rw-rw-rw-   0        0        0     1662 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_response_py3.py
--rw-rw-rw-   0        0        0     1158 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_connection_status_response.py
--rw-rw-rw-   0        0        0     1191 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_connection_status_response_py3.py
--rw-rw-rw-   0        0        0     8063 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_create.py
--rw-rw-rw-   0        0        0     8083 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_create_py3.py
--rw-rw-rw-   0        0        0     2409 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response.py
--rw-rw-rw-   0        0        0     1987 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2006 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     2661 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results.py
--rw-rw-rw-   0        0        0     2735 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2414 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_py3.py
--rw-rw-rw-   0        0        0     2206 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_results.py
--rw-rw-rw-   0        0        0     2262 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     2400 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response.py
--rw-rw-rw-   0        0        0     1971 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     1990 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1813 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1860 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2405 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1358 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_results.py
--rw-rw-rw-   0        0        0     1387 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     8385 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_edit.py
--rw-rw-rw-   0        0        0     8414 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_edit_py3.py
--rw-rw-rw-   0        0        0     3752 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child.py
--rw-rw-rw-   0        0        0     3798 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_py3.py
--rw-rw-rw-   0        0        0     4014 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_with_serial_number.py
--rw-rw-rw-   0        0        0     4065 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_with_serial_number_py3.py
--rw-rw-rw-   0        0        0     2008 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_edit.py
--rw-rw-rw-   0        0        0     2026 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_edit_py3.py
--rw-rw-rw-   0        0        0     2025 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_rate_response.py
--rw-rw-rw-   0        0        0     2020 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_rate_response_py3.py
--rw-rw-rw-   0        0        0     4081 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_request.py
--rw-rw-rw-   0        0        0     4092 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_request_py3.py
--rw-rw-rw-   0        0        0     3186 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_response.py
--rw-rw-rw-   0        0        0     3179 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_response_py3.py
--rw-rw-rw-   0        0        0     1186 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_or_meter_usage.py
--rw-rw-rw-   0        0        0     1205 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_or_meter_usage_py3.py
--rw-rw-rw-   0        0        0     1460 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_request.py
--rw-rw-rw-   0        0        0     1467 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_request_py3.py
--rw-rw-rw-   0        0        0     1148 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_response.py
--rw-rw-rw-   0        0        0     1169 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_response_py3.py
--rw-rw-rw-   0        0        0     1045 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_child.py
--rw-rw-rw-   0        0        0     1039 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_child_py3.py
--rw-rw-rw-   0        0        0     1378 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_request.py
--rw-rw-rw-   0        0        0     1375 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_request_py3.py
--rw-rw-rw-   0        0        0     1990 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_response.py
--rw-rw-rw-   0        0        0     1970 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_response_py3.py
--rw-rw-rw-   0        0        0     8130 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_response.py
--rw-rw-rw-   0        0        0     8217 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_response_py3.py
--rw-rw-rw-   0        0        0     2061 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_template_response.py
--rw-rw-rw-   0        0        0     2079 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_template_response_py3.py
--rw-rw-rw-   0        0        0     1221 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_type_child.py
--rw-rw-rw-   0        0        0     1257 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_type_child_py3.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_udf_response.py
--rw-rw-rw-   0        0        0     1356 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_udf_response_py3.py
--rw-rw-rw-   0        0        0     1991 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings.py
--rw-rw-rw-   0        0        0      870 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_class_permission.py
--rw-rw-rw-   0        0        0      877 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2040 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_py3.py
--rw-rw-rw-   0        0        0     2334 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_request.py
--rw-rw-rw-   0        0        0     2395 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_request_py3.py
--rw-rw-rw-   0        0        0     1858 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_response.py
--rw-rw-rw-   0        0        0     1919 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_response_py3.py
--rw-rw-rw-   0        0        0     2237 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts.py
--rw-rw-rw-   0        0        0     1116 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_class_permission.py
--rw-rw-rw-   0        0        0     1119 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_class_permission_py3.py
--rw-rw-rw-   0        0        0     1835 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module.py
--rw-rw-rw-   0        0        0     1865 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data.py
--rw-rw-rw-   0        0        0      744 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_class_permission.py
--rw-rw-rw-   0        0        0      752 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1915 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_py3.py
--rw-rw-rw-   0        0        0      714 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_class_permission.py
--rw-rw-rw-   0        0        0      722 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1885 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_py3.py
--rw-rw-rw-   0        0        0     2282 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_py3.py
--rw-rw-rw-   0        0        0     6206 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_processor_request.py
--rw-rw-rw-   0        0        0     6321 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_processor_request_py3.py
--rw-rw-rw-   0        0        0     2108 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings.py
--rw-rw-rw-   0        0        0      987 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_class_permission.py
--rw-rw-rw-   0        0        0      990 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2153 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_py3.py
--rw-rw-rw-   0        0        0     2217 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_response.py
--rw-rw-rw-   0        0        0     2269 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_response_py3.py
--rw-rw-rw-   0        0        0     2070 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/actionable_bill_counts.py
--rw-rw-rw-   0        0        0     2142 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/actionable_bill_counts_py3.py
--rw-rw-rw-   0        0        0      779 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/activity.py
--rw-rw-rw-   0        0        0      782 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/activity_py3.py
--rw-rw-rw-   0        0        0     3685 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_child.py
--rw-rw-rw-   0        0        0     3694 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_child_py3.py
--rw-rw-rw-   0        0        0     2541 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_lookup.py
--rw-rw-rw-   0        0        0     2574 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_lookup_py3.py
--rw-rw-rw-   0        0        0     1356 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjusted_cost_type_response.py
--rw-rw-rw-   0        0        0     1410 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjusted_cost_type_response_py3.py
--rw-rw-rw-   0        0        0     1052 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjustment_base_method_child.py
--rw-rw-rw-   0        0        0     1080 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjustment_base_method_child_py3.py
--rw-rw-rw-   0        0        0     1884 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_request.py
--rw-rw-rw-   0        0        0     1888 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_request_py3.py
--rw-rw-rw-   0        0        0     1102 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_response.py
--rw-rw-rw-   0        0        0     1108 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_response_py3.py
--rw-rw-rw-   0        0        0     1352 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison.py
--rw-rw-rw-   0        0        0     1353 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison_py3.py
--rw-rw-rw-   0        0        0     1211 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_item_rank_response.py
--rw-rw-rw-   0        0        0     1218 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_item_rank_response_py3.py
--rw-rw-rw-   0        0        0     1098 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_monthly_cap_trend_response.py
--rw-rw-rw-   0        0        0     1114 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_monthly_cap_trend_response_py3.py
--rw-rw-rw-   0        0        0     1204 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_ghg_building_rank.py
--rw-rw-rw-   0        0        0     1199 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_ghg_building_rank_py3.py
--rw-rw-rw-   0        0        0     1267 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_item_rank_with_unit_response.py
--rw-rw-rw-   0        0        0     1262 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_item_rank_with_unit_response_py3.py
--rw-rw-rw-   0        0        0     1850 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports.py
--rw-rw-rw-   0        0        0      729 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_class_permission.py
--rw-rw-rw-   0        0        0      737 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_class_permission_py3.py
--rw-rw-rw-   0        0        0     1900 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_py3.py
--rw-rw-rw-   0        0        0     1323 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_request.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_request_py3.py
--rw-rw-rw-   0        0        0     1831 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_response.py
--rw-rw-rw-   0        0        0     1854 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_response_py3.py
--rw-rw-rw-   0        0        0     1380 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_edit_request.py
--rw-rw-rw-   0        0        0     1401 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_edit_request_py3.py
--rw-rw-rw-   0        0        0     1590 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_response.py
--rw-rw-rw-   0        0        0     1614 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_response_py3.py
--rw-rw-rw-   0        0        0      834 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_user.py
--rw-rw-rw-   0        0        0      847 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_user_py3.py
--rw-rw-rw-   0        0        0     1994 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_class_permission.py
--rw-rw-rw-   0        0        0      880 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2043 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_py3.py
--rw-rw-rw-   0        0        0     1105 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_child.py
--rw-rw-rw-   0        0        0     1142 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_child_py3.py
--rw-rw-rw-   0        0        0     1057 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_request_child.py
--rw-rw-rw-   0        0        0     1075 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_request_child_py3.py
--rw-rw-rw-   0        0        0     1261 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_settings.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_settings_py3.py
--rw-rw-rw-   0        0        0     1841 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills.py
--rw-rw-rw-   0        0        0      720 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_class_permission.py
--rw-rw-rw-   0        0        0      730 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_class_permission_py3.py
--rw-rw-rw-   0        0        0     1893 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_py3.py
--rw-rw-rw-   0        0        0      980 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/assign_versions_to_step.py
--rw-rw-rw-   0        0        0     1004 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/assign_versions_to_step_py3.py
--rw-rw-rw-   0        0        0     2222 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_request.py
--rw-rw-rw-   0        0        0     2269 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_request_py3.py
--rw-rw-rw-   0        0        0     2293 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_response.py
--rw-rw-rw-   0        0        0     2340 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_response_py3.py
--rw-rw-rw-   0        0        0     1574 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_request.py
--rw-rw-rw-   0        0        0     1591 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_request_py3.py
--rw-rw-rw-   0        0        0     1860 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_response.py
--rw-rw-rw-   0        0        0     1892 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_response_py3.py
--rw-rw-rw-   0        0        0    13015 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_request.py
--rw-rw-rw-   0        0        0    13542 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_request_py3.py
--rw-rw-rw-   0        0        0    11371 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_response.py
--rw-rw-rw-   0        0        0    12003 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_response_py3.py
--rw-rw-rw-   0        0        0     1829 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine.py
--rw-rw-rw-   0        0        0      708 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_class_permission.py
--rw-rw-rw-   0        0        0      715 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_class_permission_py3.py
--rw-rw-rw-   0        0        0     1878 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_py3.py
--rw-rw-rw-   0        0        0     1588 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_log.py
--rw-rw-rw-   0        0        0     1618 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_log_py3.py
--rw-rw-rw-   0        0        0     4474 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request.py
--rw-rw-rw-   0        0        0     1032 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_baseline_bill.py
--rw-rw-rw-   0        0        0     1046 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_baseline_bill_py3.py
--rw-rw-rw-   0        0        0     4575 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_py3.py
--rw-rw-rw-   0        0        0    11293 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response.py
--rw-rw-rw-   0        0        0     3493 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_baseline_bill.py
--rw-rw-rw-   0        0        0     3559 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_baseline_bill_py3.py
--rw-rw-rw-   0        0        0    11696 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_py3.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_child.py
--rw-rw-rw-   0        0        0      886 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_child_py3.py
--rw-rw-rw-   0        0        0     4045 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_create.py
--rw-rw-rw-   0        0        0     4091 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_create_py3.py
--rw-rw-rw-   0        0        0     1376 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_edit.py
--rw-rw-rw-   0        0        0     1380 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_edit_py3.py
--rw-rw-rw-   0        0        0     5049 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_response.py
--rw-rw-rw-   0        0        0     5135 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_response_py3.py
--rw-rw-rw-   0        0        0     2159 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_settings.py
--rw-rw-rw-   0        0        0     2186 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_settings_py3.py
--rw-rw-rw-   0        0        0     2802 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_child.py
--rw-rw-rw-   0        0        0     2785 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_child_py3.py
--rw-rw-rw-   0        0        0     2527 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_settings.py
--rw-rw-rw-   0        0        0     2556 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_settings_py3.py
--rw-rw-rw-   0        0        0     1088 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_category_response.py
--rw-rw-rw-   0        0        0     1127 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_category_response_py3.py
--rw-rw-rw-   0        0        0     1433 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_edit.py
--rw-rw-rw-   0        0        0     1453 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_edit_py3.py
--rw-rw-rw-   0        0        0     1182 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_edit.py
--rw-rw-rw-   0        0        0     1184 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_edit_py3.py
--rw-rw-rw-   0        0        0     1296 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_response.py
--rw-rw-rw-   0        0        0     1298 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_response_py3.py
--rw-rw-rw-   0        0        0     1649 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value.py
--rw-rw-rw-   0        0        0     1665 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_py3.py
--rw-rw-rw-   0        0        0     1674 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_request.py
--rw-rw-rw-   0        0        0     1675 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_request_py3.py
--rw-rw-rw-   0        0        0     1796 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_values_response.py
--rw-rw-rw-   0        0        0     1832 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_values_response_py3.py
--rw-rw-rw-   0        0        0     1523 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_with_used_count_response.py
--rw-rw-rw-   0        0        0     1558 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_with_used_count_response_py3.py
--rw-rw-rw-   0        0        0     2076 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_create.py
--rw-rw-rw-   0        0        0     2098 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_create_py3.py
--rw-rw-rw-   0        0        0     2536 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_edit.py
--rw-rw-rw-   0        0        0     2562 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_edit_py3.py
--rw-rw-rw-   0        0        0     3745 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_child.py
--rw-rw-rw-   0        0        0     3863 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_child_py3.py
--rw-rw-rw-   0        0        0     7951 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_response.py
--rw-rw-rw-   0        0        0     8167 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_response_py3.py
--rw-rw-rw-   0        0        0     2574 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_statistics_response.py
--rw-rw-rw-   0        0        0     2562 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_statistics_response_py3.py
--rw-rw-rw-   0        0        0     1337 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_accrual_exclusion_request.py
--rw-rw-rw-   0        0        0     1333 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_accrual_exclusion_request_py3.py
--rw-rw-rw-   0        0        0     1006 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_approve.py
--rw-rw-rw-   0        0        0     1007 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_approve_py3.py
--rw-rw-rw-   0        0        0     1319 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_custom.py
--rw-rw-rw-   0        0        0     1322 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_custom_py3.py
--rw-rw-rw-   0        0        0      731 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_delete.py
--rw-rw-rw-   0        0        0      732 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_delete_py3.py
--rw-rw-rw-   0        0        0     1043 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_export_hold.py
--rw-rw-rw-   0        0        0     1048 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_export_hold_py3.py
--rw-rw-rw-   0        0        0     1305 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_header_update.py
--rw-rw-rw-   0        0        0     1299 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_header_update_py3.py
--rw-rw-rw-   0        0        0      943 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_historical_export.py
--rw-rw-rw-   0        0        0      939 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_historical_export_py3.py
--rw-rw-rw-   0        0        0     2018 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move.py
--rw-rw-rw-   0        0        0     1750 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_list.py
--rw-rw-rw-   0        0        0     1787 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_list_py3.py
--rw-rw-rw-   0        0        0     2045 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_py3.py
--rw-rw-rw-   0        0        0     1149 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_split.py
--rw-rw-rw-   0        0        0     1147 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_split_py3.py
--rw-rw-rw-   0        0        0      979 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_void.py
--rw-rw-rw-   0        0        0      977 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_void_py3.py
--rw-rw-rw-   0        0        0     3784 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_calendarized_history.py
--rw-rw-rw-   0        0        0     3848 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_calendarized_history_py3.py
--rw-rw-rw-   0        0        0     2248 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request.py
--rw-rw-rw-   0        0        0     2274 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request_py3.py
--rw-rw-rw-   0        0        0     2373 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response.py
--rw-rw-rw-   0        0        0     2414 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response_py3.py
--rw-rw-rw-   0        0        0     2126 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_request.py
--rw-rw-rw-   0        0        0     2145 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_request_py3.py
--rw-rw-rw-   0        0        0     2251 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_response.py
--rw-rw-rw-   0        0        0     2285 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_response_py3.py
--rw-rw-rw-   0        0        0     5406 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_create.py
--rw-rw-rw-   0        0        0     5404 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_create_py3.py
--rw-rw-rw-   0        0        0      863 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_delete_action_result.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_delete_action_result_py3.py
--rw-rw-rw-   0        0        0     6222 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_edit.py
--rw-rw-rw-   0        0        0     6230 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_edit_py3.py
--rw-rw-rw-   0        0        0     1601 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line.py
--rw-rw-rw-   0        0        0     1058 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_child.py
--rw-rw-rw-   0        0        0     1055 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_child_py3.py
--rw-rw-rw-   0        0        0     1601 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_py3.py
--rw-rw-rw-   0        0        0     1233 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_with_noun_child.py
--rw-rw-rw-   0        0        0     1226 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_with_noun_child_py3.py
--rw-rw-rw-   0        0        0     1894 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_meter_child.py
--rw-rw-rw-   0        0        0     1923 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_meter_child_py3.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_observation_type_child.py
--rw-rw-rw-   0        0        0     1392 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_observation_type_child_py3.py
--rw-rw-rw-   0        0        0     8971 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_response.py
--rw-rw-rw-   0        0        0     9045 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_response_py3.py
--rw-rw-rw-   0        0        0     1869 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export.py
--rw-rw-rw-   0        0        0     1555 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_options.py
--rw-rw-rw-   0        0        0     1571 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_options_py3.py
--rw-rw-rw-   0        0        0     1880 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_py3.py
--rw-rw-rw-   0        0        0      918 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_child.py
--rw-rw-rw-   0        0        0      927 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_child_py3.py
--rw-rw-rw-   0        0        0     3433 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update.py
--rw-rw-rw-   0        0        0     1379 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_account_period_child.py
--rw-rw-rw-   0        0        0     1390 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_account_period_child_py3.py
--rw-rw-rw-   0        0        0     1310 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_begin_date_child.py
--rw-rw-rw-   0        0        0     1312 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_begin_date_child_py3.py
--rw-rw-rw-   0        0        0     1252 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_billing_period_child.py
--rw-rw-rw-   0        0        0     1263 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_billing_period_child_py3.py
--rw-rw-rw-   0        0        0     1360 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_control_code_child.py
--rw-rw-rw-   0        0        0     1369 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_control_code_child_py3.py
--rw-rw-rw-   0        0        0     1275 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_due_date_child.py
--rw-rw-rw-   0        0        0     1275 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_due_date_child_py3.py
--rw-rw-rw-   0        0        0     1292 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_end_date_child.py
--rw-rw-rw-   0        0        0     1292 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_end_date_child_py3.py
--rw-rw-rw-   0        0        0     1212 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_estimated_child.py
--rw-rw-rw-   0        0        0     1219 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_estimated_child_py3.py
--rw-rw-rw-   0        0        0     1378 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_invoice_number_child.py
--rw-rw-rw-   0        0        0     1389 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_invoice_number_child_py3.py
--rw-rw-rw-   0        0        0     3385 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_py3.py
--rw-rw-rw-   0        0        0     1329 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_statement_date_child.py
--rw-rw-rw-   0        0        0     1335 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_statement_date_child_py3.py
--rw-rw-rw-   0        0        0      881 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_workflow_child.py
--rw-rw-rw-   0        0        0      895 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_workflow_child_py3.py
--rw-rw-rw-   0        0        0     3431 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_history_response.py
--rw-rw-rw-   0        0        0     3451 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_history_response_py3.py
--rw-rw-rw-   0        0        0      704 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_id_response.py
--rw-rw-rw-   0        0        0      714 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_id_response_py3.py
--rw-rw-rw-   0        0        0     9204 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_column_mapping.py
--rw-rw-rw-   0        0        0     9494 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_column_mapping_py3.py
--rw-rw-rw-   0        0        0     2051 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_observation.py
--rw-rw-rw-   0        0        0     2059 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_observation_py3.py
--rw-rw-rw-   0        0        0     1333 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_request.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_request_py3.py
--rw-rw-rw-   0        0        0     1634 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_response.py
--rw-rw-rw-   0        0        0     1647 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_response_py3.py
--rw-rw-rw-   0        0        0     2737 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_request.py
--rw-rw-rw-   0        0        0     2751 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_request_py3.py
--rw-rw-rw-   0        0        0      920 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_workflow_settings.py
--rw-rw-rw-   0        0        0      937 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_workflow_settings_py3.py
--rw-rw-rw-   0        0        0     1868 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator.py
--rw-rw-rw-   0        0        0      747 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_class_permission.py
--rw-rw-rw-   0        0        0      757 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_class_permission_py3.py
--rw-rw-rw-   0        0        0     1920 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_py3.py
--rw-rw-rw-   0        0        0     2173 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_create.py
--rw-rw-rw-   0        0        0     2190 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_create_py3.py
--rw-rw-rw-   0        0        0     2701 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_edit.py
--rw-rw-rw-   0        0        0     2722 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_edit_py3.py
--rw-rw-rw-   0        0        0     1339 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_create.py
--rw-rw-rw-   0        0        0     1337 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_create_py3.py
--rw-rw-rw-   0        0        0     1329 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_edit.py
--rw-rw-rw-   0        0        0     1327 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_edit_py3.py
--rw-rw-rw-   0        0        0     1461 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_file_response.py
--rw-rw-rw-   0        0        0     1476 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_file_response_py3.py
--rw-rw-rw-   0        0        0     3854 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_item.py
--rw-rw-rw-   0        0        0     3854 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_item_py3.py
--rw-rw-rw-   0        0        0     1569 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_response.py
--rw-rw-rw-   0        0        0     1591 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_response_py3.py
--rw-rw-rw-   0        0        0    12793 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_response.py
--rw-rw-rw-   0        0        0    12915 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_response_py3.py
--rw-rw-rw-   0        0        0     1391 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal.py
--rw-rw-rw-   0        0        0     1420 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_py3.py
--rw-rw-rw-   0        0        0     1224 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_request.py
--rw-rw-rw-   0        0        0     1226 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_request_py3.py
--rw-rw-rw-   0        0        0     2225 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request.py
--rw-rw-rw-   0        0        0     2257 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request_py3.py
--rw-rw-rw-   0        0        0     2350 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response.py
--rw-rw-rw-   0        0        0     2397 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response_py3.py
--rw-rw-rw-   0        0        0     2497 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_request.py
--rw-rw-rw-   0        0        0     2531 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_request_py3.py
--rw-rw-rw-   0        0        0     2020 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_response.py
--rw-rw-rw-   0        0        0     2048 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_response_py3.py
--rw-rw-rw-   0        0        0     1555 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_parent_details_response.py
--rw-rw-rw-   0        0        0     1584 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_parent_details_response_py3.py
--rw-rw-rw-   0        0        0     1388 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_place_size_child.py
--rw-rw-rw-   0        0        0     1386 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_place_size_child_py3.py
--rw-rw-rw-   0        0        0     1294 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport.py
--rw-rw-rw-   0        0        0      990 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_options.py
--rw-rw-rw-   0        0        0      999 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_options_py3.py
--rw-rw-rw-   0        0        0     1293 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_py3.py
--rw-rw-rw-   0        0        0     1341 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_usage.py
--rw-rw-rw-   0        0        0     1361 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_usage_py3.py
--rw-rw-rw-   0        0        0     2125 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_account_child.py
--rw-rw-rw-   0        0        0     2139 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_account_child_py3.py
--rw-rw-rw-   0        0        0     1955 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_address_child.py
--rw-rw-rw-   0        0        0     1959 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_address_child_py3.py
--rw-rw-rw-   0        0        0     2282 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_meter_child.py
--rw-rw-rw-   0        0        0     2279 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_meter_child_py3.py
--rw-rw-rw-   0        0        0    15009 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_response.py
--rw-rw-rw-   0        0        0    15189 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_response_py3.py
--rw-rw-rw-   0        0        0     1311 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_vendor_child.py
--rw-rw-rw-   0        0        0     1323 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_vendor_child_py3.py
--rw-rw-rw-   0        0        0     1997 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings.py
--rw-rw-rw-   0        0        0      876 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_class_permission.py
--rw-rw-rw-   0        0        0      883 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2046 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_py3.py
--rw-rw-rw-   0        0        0      887 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_child.py
--rw-rw-rw-   0        0        0      887 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_child_py3.py
--rw-rw-rw-   0        0        0     1149 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_delta_child.py
--rw-rw-rw-   0        0        0     1148 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_delta_child_py3.py
--rw-rw-rw-   0        0        0     2300 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_child.py
--rw-rw-rw-   0        0        0     2354 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_child_py3.py
--rw-rw-rw-   0        0        0     1355 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_delta_child.py
--rw-rw-rw-   0        0        0     1353 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_delta_child_py3.py
--rw-rw-rw-   0        0        0      884 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_child.py
--rw-rw-rw-   0        0        0      883 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_child_py3.py
--rw-rw-rw-   0        0        0     1097 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_delta_child.py
--rw-rw-rw-   0        0        0     1095 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_delta_child_py3.py
--rw-rw-rw-   0        0        0     2402 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches.py
--rw-rw-rw-   0        0        0     1281 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_class_permission.py
--rw-rw-rw-   0        0        0     1283 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_class_permission_py3.py
--rw-rw-rw-   0        0        0     2446 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_py3.py
--rw-rw-rw-   0        0        0     1826 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module.py
--rw-rw-rw-   0        0        0      705 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_class_permission.py
--rw-rw-rw-   0        0        0      713 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1876 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_py3.py
--rw-rw-rw-   0        0        0     1804 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_overdue_from_vendor_response.py
--rw-rw-rw-   0        0        0     1799 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_overdue_from_vendor_response_py3.py
--rw-rw-rw-   0        0        0     3173 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_child.py
--rw-rw-rw-   0        0        0     3209 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_child_py3.py
--rw-rw-rw-   0        0        0     3182 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_response.py
--rw-rw-rw-   0        0        0     3169 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_response_py3.py
--rw-rw-rw-   0        0        0     2285 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions.py
--rw-rw-rw-   0        0        0     1164 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_class_permission.py
--rw-rw-rw-   0        0        0     1167 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_class_permission_py3.py
--rw-rw-rw-   0        0        0     2330 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_py3.py
--rw-rw-rw-   0        0        0     2147 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups.py
--rw-rw-rw-   0        0        0     1026 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_class_permission.py
--rw-rw-rw-   0        0        0     1032 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_class_permission_py3.py
--rw-rw-rw-   0        0        0     2195 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_py3.py
--rw-rw-rw-   0        0        0     1865 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module.py
--rw-rw-rw-   0        0        0     1895 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data.py
--rw-rw-rw-   0        0        0      774 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission.py
--rw-rw-rw-   0        0        0      782 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1945 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_py3.py
--rw-rw-rw-   0        0        0     1913 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data.py
--rw-rw-rw-   0        0        0      792 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission.py
--rw-rw-rw-   0        0        0      800 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1963 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_py3.py
--rw-rw-rw-   0        0        0      744 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_class_permission.py
--rw-rw-rw-   0        0        0      752 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1916 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data.py
--rw-rw-rw-   0        0        0      795 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission.py
--rw-rw-rw-   0        0        0      803 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1966 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_py3.py
--rw-rw-rw-   0        0        0     1907 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data.py
--rw-rw-rw-   0        0        0      786 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission.py
--rw-rw-rw-   0        0        0      794 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1957 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_py3.py
--rw-rw-rw-   0        0        0     1915 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_py3.py
--rw-rw-rw-   0        0        0     1886 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings.py
--rw-rw-rw-   0        0        0      765 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_class_permission.py
--rw-rw-rw-   0        0        0      773 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_class_permission_py3.py
--rw-rw-rw-   0        0        0     1936 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_py3.py
--rw-rw-rw-   0        0        0     1907 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability.py
--rw-rw-rw-   0        0        0      786 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission.py
--rw-rw-rw-   0        0        0      794 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission_py3.py
--rw-rw-rw-   0        0        0     1957 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_py3.py
--rw-rw-rw-   0        0        0     2288 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations.py
--rw-rw-rw-   0        0        0     1167 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_class_permission.py
--rw-rw-rw-   0        0        0     1170 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_class_permission_py3.py
--rw-rw-rw-   0        0        0     2333 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_py3.py
--rw-rw-rw-   0        0        0     1303 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_baseline_processor_request.py
--rw-rw-rw-   0        0        0     1327 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_baseline_processor_request_py3.py
--rw-rw-rw-   0        0        0     4384 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_meter_cost_avoidance_settings.py
--rw-rw-rw-   0        0        0     4497 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_meter_cost_avoidance_settings_py3.py
--rw-rw-rw-   0        0        0     3123 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculate_savings_request.py
--rw-rw-rw-   0        0        0     3197 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculate_savings_request_py3.py
--rw-rw-rw-   0        0        0     2972 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_request.py
--rw-rw-rw-   0        0        0     3052 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_request_py3.py
--rw-rw-rw-   0        0        0     2451 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_response.py
--rw-rw-rw-   0        0        0     2503 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_response_py3.py
--rw-rw-rw-   0        0        0     1488 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_request.py
--rw-rw-rw-   0        0        0     1524 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_request_py3.py
--rw-rw-rw-   0        0        0     1480 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_response.py
--rw-rw-rw-   0        0        0     1517 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_response_py3.py
--rw-rw-rw-   0        0        0     2326 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_details_response.py
--rw-rw-rw-   0        0        0     2313 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_details_response_py3.py
--rw-rw-rw-   0        0        0     2437 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_request.py
--rw-rw-rw-   0        0        0     2496 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_request_py3.py
--rw-rw-rw-   0        0        0     2377 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_response.py
--rw-rw-rw-   0        0        0     2437 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_response_py3.py
--rw-rw-rw-   0        0        0     1015 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_request.py
--rw-rw-rw-   0        0        0     1011 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_request_py3.py
--rw-rw-rw-   0        0        0     1118 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_response.py
--rw-rw-rw-   0        0        0     1114 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_response_py3.py
--rw-rw-rw-   0        0        0      819 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_request.py
--rw-rw-rw-   0        0        0      820 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_request_py3.py
--rw-rw-rw-   0        0        0      888 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_response.py
--rw-rw-rw-   0        0        0      902 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_response_py3.py
--rw-rw-rw-   0        0        0     1116 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_sum_request.py
--rw-rw-rw-   0        0        0     1122 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_sum_request_py3.py
--rw-rw-rw-   0        0        0     1351 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child.py
--rw-rw-rw-   0        0        0     1368 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_py3.py
--rw-rw-rw-   0        0        0     1770 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_with_observation_type.py
--rw-rw-rw-   0        0        0     1769 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_with_observation_type_py3.py
--rw-rw-rw-   0        0        0     2674 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_create.py
--rw-rw-rw-   0        0        0     2713 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_create_py3.py
--rw-rw-rw-   0        0        0     2828 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_edit.py
--rw-rw-rw-   0        0        0     2872 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_edit_py3.py
--rw-rw-rw-   0        0        0     1556 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_latest_reading.py
--rw-rw-rw-   0        0        0     1571 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_latest_reading_py3.py
--rw-rw-rw-   0        0        0     3383 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_response.py
--rw-rw-rw-   0        0        0     3452 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_response_py3.py
--rw-rw-rw-   0        0        0     2747 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_request.py
--rw-rw-rw-   0        0        0     2751 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_request_py3.py
--rw-rw-rw-   0        0        0     2309 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_response.py
--rw-rw-rw-   0        0        0     2320 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_response_py3.py
--rw-rw-rw-   0        0        0     3091 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_with_begin_date_request.py
--rw-rw-rw-   0        0        0     3092 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_with_begin_date_request_py3.py
--rw-rw-rw-   0        0        0     2867 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings.py
--rw-rw-rw-   0        0        0     1240 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_aggregations.py
--rw-rw-rw-   0        0        0     1254 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_aggregations_py3.py
--rw-rw-rw-   0        0        0      982 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_splits.py
--rw-rw-rw-   0        0        0      990 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_splits_py3.py
--rw-rw-rw-   0        0        0     2880 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_py3.py
--rw-rw-rw-   0        0        0     2563 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_without_filters.py
--rw-rw-rw-   0        0        0     2582 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_without_filters_py3.py
--rw-rw-rw-   0        0        0     1862 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals.py
--rw-rw-rw-   0        0        0      741 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_class_permission.py
--rw-rw-rw-   0        0        0      751 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_class_permission_py3.py
--rw-rw-rw-   0        0        0     1914 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_py3.py
--rw-rw-rw-   0        0        0      936 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_request.py
--rw-rw-rw-   0        0        0      941 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_request_py3.py
--rw-rw-rw-   0        0        0     4421 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_response.py
--rw-rw-rw-   0        0        0     4471 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_response_py3.py
--rw-rw-rw-   0        0        0     5239 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_version_response.py
--rw-rw-rw-   0        0        0     5292 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_version_response_py3.py
--rw-rw-rw-   0        0        0     1122 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_base.py
--rw-rw-rw-   0        0        0     1163 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_base_py3.py
--rw-rw-rw-   0        0        0     1713 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_create.py
--rw-rw-rw-   0        0        0     1747 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_create_py3.py
--rw-rw-rw-   0        0        0     2045 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_child.py
--rw-rw-rw-   0        0        0     2038 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_child_py3.py
--rw-rw-rw-   0        0        0     1238 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_response.py
--rw-rw-rw-   0        0        0     1254 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_response_py3.py
--rw-rw-rw-   0        0        0     1518 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_split_child.py
--rw-rw-rw-   0        0        0     1518 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_split_child_py3.py
--rw-rw-rw-   0        0        0     1766 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_edit.py
--rw-rw-rw-   0        0        0     1800 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_edit_py3.py
--rw-rw-rw-   0        0        0     1497 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_response.py
--rw-rw-rw-   0        0        0     1550 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_response_py3.py
--rw-rw-rw-   0        0        0     1228 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_settings.py
--rw-rw-rw-   0        0        0     1261 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_settings_py3.py
--rw-rw-rw-   0        0        0     2300 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step.py
--rw-rw-rw-   0        0        0     2703 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_child.py
--rw-rw-rw-   0        0        0     2831 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_child_py3.py
--rw-rw-rw-   0        0        0     2282 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_create.py
--rw-rw-rw-   0        0        0     2353 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_create_py3.py
--rw-rw-rw-   0        0        0     2998 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_edit.py
--rw-rw-rw-   0        0        0     3088 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_edit_py3.py
--rw-rw-rw-   0        0        0     2422 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_py3.py
--rw-rw-rw-   0        0        0     1964 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks.py
--rw-rw-rw-   0        0        0      843 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_class_permission.py
--rw-rw-rw-   0        0        0      849 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_class_permission_py3.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module.py
--rw-rw-rw-   0        0        0      723 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_class_permission.py
--rw-rw-rw-   0        0        0      731 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1894 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_py3.py
--rw-rw-rw-   0        0        0     2012 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_py3.py
--rw-rw-rw-   0        0        0      837 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/claim.py
--rw-rw-rw-   0        0        0      847 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/claim_py3.py
--rw-rw-rw-   0        0        0     1872 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_child.py
--rw-rw-rw-   0        0        0     1371 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_child_py3.py
--rw-rw-rw-   0        0        0     1838 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response.py
--rw-rw-rw-   0        0        0     1981 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2000 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1819 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1866 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     1833 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1364 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_results.py
--rw-rw-rw-   0        0        0     1393 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1915 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_py3.py
--rw-rw-rw-   0        0        0     1249 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_value_comparison.py
--rw-rw-rw-   0        0        0     1257 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_value_comparison_py3.py
--rw-rw-rw-   0        0        0     1202 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/contact_child.py
--rw-rw-rw-   0        0        0     1206 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/contact_child_py3.py
--rw-rw-rw-   0        0        0     1002 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_from_meter_response.py
--rw-rw-rw-   0        0        0     1009 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_from_meter_response_py3.py
--rw-rw-rw-   0        0        0     1732 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_meter_request.py
--rw-rw-rw-   0        0        0     1737 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_meter_request_py3.py
--rw-rw-rw-   0        0        0     3353 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_settings.py
--rw-rw-rw-   0        0        0     3465 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_settings_py3.py
--rw-rw-rw-   0        0        0     4158 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_task.py
--rw-rw-rw-   0        0        0     4154 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_task_py3.py
--rw-rw-rw-   0        0        0     2421 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_account_child.py
--rw-rw-rw-   0        0        0     2482 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_account_child_py3.py
--rw-rw-rw-   0        0        0     1197 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_child.py
--rw-rw-rw-   0        0        0     1230 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_child_py3.py
--rw-rw-rw-   0        0        0     2098 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_create.py
--rw-rw-rw-   0        0        0     2123 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_create_py3.py
--rw-rw-rw-   0        0        0     2508 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response.py
--rw-rw-rw-   0        0        0     2002 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2021 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     2670 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results.py
--rw-rw-rw-   0        0        0     2744 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2525 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_py3.py
--rw-rw-rw-   0        0        0     2215 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_results.py
--rw-rw-rw-   0        0        0     2271 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     2499 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response.py
--rw-rw-rw-   0        0        0     1986 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2005 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1822 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1869 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2516 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1367 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_results.py
--rw-rw-rw-   0        0        0     1396 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1905 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_response.py
--rw-rw-rw-   0        0        0     1925 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_response_py3.py
--rw-rw-rw-   0        0        0     2246 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers.py
--rw-rw-rw-   0        0        0     1125 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_class_permission.py
--rw-rw-rw-   0        0        0     1128 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_class_permission_py3.py
--rw-rw-rw-   0        0        0     2291 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_py3.py
--rw-rw-rw-   0        0        0     1000 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_child.py
--rw-rw-rw-   0        0        0     1021 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_child_py3.py
--rw-rw-rw-   0        0        0     1327 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_unit.py
--rw-rw-rw-   0        0        0     1378 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_unit_py3.py
--rw-rw-rw-   0        0        0     1203 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/country.py
--rw-rw-rw-   0        0        0     1220 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/country_py3.py
--rw-rw-rw-   0        0        0     1404 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_template_from_bill.py
--rw-rw-rw-   0        0        0     1411 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_template_from_bill_py3.py
--rw-rw-rw-   0        0        0     1074 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_utility_platform_meter.py
--rw-rw-rw-   0        0        0     1082 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_utility_platform_meter_py3.py
--rw-rw-rw-   0        0        0     1131 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_child.py
--rw-rw-rw-   0        0        0     1155 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_child_py3.py
--rw-rw-rw-   0        0        0     1328 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_response.py
--rw-rw-rw-   0        0        0     1346 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_response_py3.py
--rw-rw-rw-   0        0        0     1871 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator.py
--rw-rw-rw-   0        0        0      750 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_class_permission.py
--rw-rw-rw-   0        0        0      760 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_class_permission_py3.py
--rw-rw-rw-   0        0        0     1923 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_py3.py
--rw-rw-rw-   0        0        0     1859 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module.py
--rw-rw-rw-   0        0        0      738 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_class_permission.py
--rw-rw-rw-   0        0        0      746 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1909 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_py3.py
--rw-rw-rw-   0        0        0     1646 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_copy.py
--rw-rw-rw-   0        0        0     1665 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_copy_py3.py
--rw-rw-rw-   0        0        0     1815 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_create.py
--rw-rw-rw-   0        0        0     1825 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_create_py3.py
--rw-rw-rw-   0        0        0     2036 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_edit.py
--rw-rw-rw-   0        0        0     2041 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_edit_py3.py
--rw-rw-rw-   0        0        0     2766 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings.py
--rw-rw-rw-   0        0        0     2986 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_edit.py
--rw-rw-rw-   0        0        0     3024 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_edit_py3.py
--rw-rw-rw-   0        0        0     2809 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_py3.py
--rw-rw-rw-   0        0        0     3497 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_response.py
--rw-rw-rw-   0        0        0     3516 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_response_py3.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release.py
--rw-rw-rw-   0        0        0     1130 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_meta_data.py
--rw-rw-rw-   0        0        0     1158 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_meta_data_py3.py
--rw-rw-rw-   0        0        0     1639 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_no_file_request.py
--rw-rw-rw-   0        0        0     1652 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_no_file_request_py3.py
--rw-rw-rw-   0        0        0     1874 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_py3.py
--rw-rw-rw-   0        0        0     1994 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_request.py
--rw-rw-rw-   0        0        0     2016 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_request_py3.py
--rw-rw-rw-   0        0        0     1110 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_state.py
--rw-rw-rw-   0        0        0     1123 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_state_py3.py
--rw-rw-rw-   0        0        0     1399 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_status.py
--rw-rw-rw-   0        0        0     1454 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_status_py3.py
--rw-rw-rw-   0        0        0     1287 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_type_response.py
--rw-rw-rw-   0        0        0     1314 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_type_response_py3.py
--rw-rw-rw-   0        0        0      987 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/delete_reading_response.py
--rw-rw-rw-   0        0        0      992 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/delete_reading_response_py3.py
--rw-rw-rw-   0        0        0     1877 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_meter_child.py
--rw-rw-rw-   0        0        0     1896 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_meter_child_py3.py
--rw-rw-rw-   0        0        0     1863 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_response.py
--rw-rw-rw-   0        0        0     1870 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_response_py3.py
--rw-rw-rw-   0        0        0      750 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_base.py
--rw-rw-rw-   0        0        0      764 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_base_py3.py
--rw-rw-rw-   0        0        0     1148 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_to_bills_request.py
--rw-rw-rw-   0        0        0     1157 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_to_bills_request_py3.py
--rw-rw-rw-   0        0        0     3951 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_configuration.py
--rw-rw-rw-   0        0        0     3976 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_configuration_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings.py
--rw-rw-rw-   0        0        0      762 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_class_permission.py
--rw-rw-rw-   0        0        0      772 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     1935 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_py3.py
--rw-rw-rw-   0        0        0     3340 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_manage.py
--rw-rw-rw-   0        0        0     3360 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_manage_py3.py
--rw-rw-rw-   0        0        0     2589 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_response.py
--rw-rw-rw-   0        0        0     2602 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_response_py3.py
--rw-rw-rw-   0        0        0     2183 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request.py
--rw-rw-rw-   0        0        0     2196 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request_py3.py
--rw-rw-rw-   0        0        0     2213 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response.py
--rw-rw-rw-   0        0        0     2241 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response_py3.py
--rw-rw-rw-   0        0        0     1132 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_list_request.py
--rw-rw-rw-   0        0        0     1143 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_list_request_py3.py
--rw-rw-rw-   0        0        0     2193 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split.py
--rw-rw-rw-   0        0        0     2235 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_py3.py
--rw-rw-rw-   0        0        0     1640 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_response.py
--rw-rw-rw-   0        0        0     1689 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_response_py3.py
--rw-rw-rw-   0        0        0     1247 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/email_properties.py
--rw-rw-rw-   0        0        0     1245 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/email_properties_py3.py
--rw-rw-rw-   0        0        0      950 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_cap_options_energy_cap_id_options.py
--rw-rw-rw-   0        0        0      969 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_cap_options_energy_cap_id_options_py3.py
--rw-rw-rw-   0        0        0     4814 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_create.py
--rw-rw-rw-   0        0        0     4938 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_create_py3.py
--rw-rw-rw-   0        0        0     5564 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_edit.py
--rw-rw-rw-   0        0        0     5688 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_edit_py3.py
--rw-rw-rw-   0        0        0     1098 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_place_child.py
--rw-rw-rw-   0        0        0     1113 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_place_child_py3.py
--rw-rw-rw-   0        0        0     4719 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_response.py
--rw-rw-rw-   0        0        0     4795 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_response_py3.py
--rw-rw-rw-   0        0        0     1369 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type.py
--rw-rw-rw-   0        0        0     1686 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_create.py
--rw-rw-rw-   0        0        0     1719 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_create_py3.py
--rw-rw-rw-   0        0        0     1426 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_py3.py
--rw-rw-rw-   0        0        0     1036 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_child.py
--rw-rw-rw-   0        0        0     1061 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_child_py3.py
--rw-rw-rw-   0        0        0     1375 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_unit.py
--rw-rw-rw-   0        0        0     1432 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_unit_py3.py
--rw-rw-rw-   0        0        0     1861 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping.py
--rw-rw-rw-   0        0        0     1693 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child.py
--rw-rw-rw-   0        0        0     1735 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child_py3.py
--rw-rw-rw-   0        0        0     1912 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_py3.py
--rw-rw-rw-   0        0        0     2042 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_child.py
--rw-rw-rw-   0        0        0     2065 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_child_py3.py
--rw-rw-rw-   0        0        0     1256 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_request.py
--rw-rw-rw-   0        0        0     1265 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_request_py3.py
--rw-rw-rw-   0        0        0     2593 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_hierarchy_response.py
--rw-rw-rw-   0        0        0     2643 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_hierarchy_response_py3.py
--rw-rw-rw-   0        0        0     1358 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_request.py
--rw-rw-rw-   0        0        0     1368 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_request_py3.py
--rw-rw-rw-   0        0        0     1224 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_response.py
--rw-rw-rw-   0        0        0     1226 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_response_py3.py
--rw-rw-rw-   0        0        0     1708 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_request.py
--rw-rw-rw-   0        0        0     1711 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_request_py3.py
--rw-rw-rw-   0        0        0     3015 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_response.py
--rw-rw-rw-   0        0        0     3150 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_response_py3.py
--rw-rw-rw-   0        0        0     1779 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_child.py
--rw-rw-rw-   0        0        0     1830 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_child_py3.py
--rw-rw-rw-   0        0        0     2066 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_response.py
--rw-rw-rw-   0        0        0     2096 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_response_py3.py
--rw-rw-rw-   0        0        0     1760 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_meter.py
--rw-rw-rw-   0        0        0     1775 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_meter_py3.py
--rw-rw-rw-   0        0        0     2426 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_property.py
--rw-rw-rw-   0        0        0     2468 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_property_py3.py
--rw-rw-rw-   0        0        0     1502 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_rating_child.py
--rw-rw-rw-   0        0        0     1535 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_rating_child_py3.py
--rw-rw-rw-   0        0        0     1506 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_request.py
--rw-rw-rw-   0        0        0     1534 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_request_py3.py
--rw-rw-rw-   0        0        0     3612 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_response.py
--rw-rw-rw-   0        0        0     3791 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_response_py3.py
--rw-rw-rw-   0        0        0     1417 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_place_child.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_place_child_py3.py
--rw-rw-rw-   0        0        0     1187 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_request.py
--rw-rw-rw-   0        0        0     1186 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_request_py3.py
--rw-rw-rw-   0        0        0     1040 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_place_child.py
--rw-rw-rw-   0        0        0     1045 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_place_child_py3.py
--rw-rw-rw-   0        0        0     3549 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_response.py
--rw-rw-rw-   0        0        0     3637 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_response_py3.py
--rw-rw-rw-   0        0        0     1994 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_class_permission.py
--rw-rw-rw-   0        0        0      879 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_class_permission_py3.py
--rw-rw-rw-   0        0        0     2042 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_py3.py
--rw-rw-rw-   0        0        0      851 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/environment.py
--rw-rw-rw-   0        0        0      858 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/environment_py3.py
--rw-rw-rw-   0        0        0     1581 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/estimated.py
--rw-rw-rw-   0        0        0     1588 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/estimated_py3.py
--rw-rw-rw-   0        0        0     2096 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills.py
--rw-rw-rw-   0        0        0      975 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_class_permission.py
--rw-rw-rw-   0        0        0      978 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_class_permission_py3.py
--rw-rw-rw-   0        0        0     2141 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_py3.py
--rw-rw-rw-   0        0        0      920 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_format_child.py
--rw-rw-rw-   0        0        0      943 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_format_child_py3.py
--rw-rw-rw-   0        0        0     1835 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold.py
--rw-rw-rw-   0        0        0      714 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_class_permission.py
--rw-rw-rw-   0        0        0      724 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_class_permission_py3.py
--rw-rw-rw-   0        0        0     1887 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_py3.py
--rw-rw-rw-   0        0        0     1840 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_child.py
--rw-rw-rw-   0        0        0     1855 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_child_py3.py
--rw-rw-rw-   0        0        0      946 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_settings.py
--rw-rw-rw-   0        0        0      971 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_settings_py3.py
--rw-rw-rw-   0        0        0     2261 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects.py
--rw-rw-rw-   0        0        0     1140 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_class_permission.py
--rw-rw-rw-   0        0        0     1143 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_class_permission_py3.py
--rw-rw-rw-   0        0        0     2306 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_py3.py
--rw-rw-rw-   0        0        0     2119 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_reading_response.py
--rw-rw-rw-   0        0        0     2173 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_reading_response_py3.py
--rw-rw-rw-   0        0        0     1245 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_readings.py
--rw-rw-rw-   0        0        0     1241 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_readings_py3.py
--rw-rw-rw-   0        0        0     1850 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/file_data_type_response.py
--rw-rw-rw-   0        0        0     1908 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/file_data_type_response_py3.py
--rw-rw-rw-   0        0        0      685 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_data_response.py
--rw-rw-rw-   0        0        0      693 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_data_response_py3.py
--rw-rw-rw-   0        0        0     1371 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_edit.py
--rw-rw-rw-   0        0        0     1369 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_edit_py3.py
--rw-rw-rw-   0        0        0     3278 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_response.py
--rw-rw-rw-   0        0        0     3307 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_response_py3.py
--rw-rw-rw-   0        0        0      910 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_amount_response.py
--rw-rw-rw-   0        0        0      912 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_amount_response_py3.py
--rw-rw-rw-   0        0        0     1342 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_demand_request.py
--rw-rw-rw-   0        0        0     1355 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_demand_request_py3.py
--rw-rw-rw-   0        0        0     2080 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage.py
--rw-rw-rw-   0        0        0     2112 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_py3.py
--rw-rw-rw-   0        0        0     1628 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_response.py
--rw-rw-rw-   0        0        0     1663 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_response_py3.py
--rw-rw-rw-   0        0        0     1312 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_unit_cost_request.py
--rw-rw-rw-   0        0        0     1315 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_unit_cost_request_py3.py
--rw-rw-rw-   0        0        0     1306 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_use_request.py
--rw-rw-rw-   0        0        0     1316 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_use_request_py3.py
--rw-rw-rw-   0        0        0      979 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_action_child.py
--rw-rw-rw-   0        0        0     1004 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_action_child_py3.py
--rw-rw-rw-   0        0        0     2886 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_edit.py
--rw-rw-rw-   0        0        0     2930 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_edit_py3.py
--rw-rw-rw-   0        0        0     1765 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_event_child.py
--rw-rw-rw-   0        0        0     1777 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_event_child_py3.py
--rw-rw-rw-   0        0        0     1587 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_issue_type_child.py
--rw-rw-rw-   0        0        0     1650 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_issue_type_child_py3.py
--rw-rw-rw-   0        0        0      999 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_list_action.py
--rw-rw-rw-   0        0        0     1005 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_list_action_py3.py
--rw-rw-rw-   0        0        0     3186 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_response.py
--rw-rw-rw-   0        0        0     3183 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_response_py3.py
--rw-rw-rw-   0        0        0      979 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_status_child.py
--rw-rw-rw-   0        0        0     1004 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_status_child_py3.py
--rw-rw-rw-   0        0        0      945 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_child.py
--rw-rw-rw-   0        0        0      966 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_child_py3.py
--rw-rw-rw-   0        0        0     1090 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_create.py
--rw-rw-rw-   0        0        0     1102 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_create_py3.py
--rw-rw-rw-   0        0        0     2519 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget.py
--rw-rw-rw-   0        0        0     3784 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_child.py
--rw-rw-rw-   0        0        0     3832 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_child_py3.py
--rw-rw-rw-   0        0        0     2560 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_py3.py
--rw-rw-rw-   0        0        0     1973 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items.py
--rw-rw-rw-   0        0        0      852 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_class_permission.py
--rw-rw-rw-   0        0        0      859 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_class_permission_py3.py
--rw-rw-rw-   0        0        0     2022 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_py3.py
--rw-rw-rw-   0        0        0     2265 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split.py
--rw-rw-rw-   0        0        0     2297 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_py3.py
--rw-rw-rw-   0        0        0     1913 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_response.py
--rw-rw-rw-   0        0        0     1958 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_response_py3.py
--rw-rw-rw-   0        0        0     1463 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_child.py
--rw-rw-rw-   0        0        0     1474 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_child_py3.py
--rw-rw-rw-   0        0        0     1405 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_request.py
--rw-rw-rw-   0        0        0     1406 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_request_py3.py
--rw-rw-rw-   0        0        0     1893 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_response.py
--rw-rw-rw-   0        0        0     1904 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_response_py3.py
--rw-rw-rw-   0        0        0     2209 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/frequency.py
--rw-rw-rw-   0        0        0     2269 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/frequency_py3.py
--rw-rw-rw-   0        0        0     1191 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_child.py
--rw-rw-rw-   0        0        0     1233 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_child_py3.py
--rw-rw-rw-   0        0        0     1513 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_request.py
--rw-rw-rw-   0        0        0     1521 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_request_py3.py
--rw-rw-rw-   0        0        0     1308 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_response.py
--rw-rw-rw-   0        0        0     1335 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_response_py3.py
--rw-rw-rw-   0        0        0     2281 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_request.py
--rw-rw-rw-   0        0        0     2309 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_request_py3.py
--rw-rw-rw-   0        0        0     1515 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_response.py
--rw-rw-rw-   0        0        0     1535 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_response_py3.py
--rw-rw-rw-   0        0        0      896 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_count.py
--rw-rw-rw-   0        0        0      907 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_count_py3.py
--rw-rw-rw-   0        0        0     3365 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_building_rank.py
--rw-rw-rw-   0        0        0     3411 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_building_rank_py3.py
--rw-rw-rw-   0        0        0     1310 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_carbon_footprint_response.py
--rw-rw-rw-   0        0        0     1316 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_carbon_footprint_response_py3.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_factor.py
--rw-rw-rw-   0        0        0     1433 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_factor_py3.py
--rw-rw-rw-   0        0        0     1375 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_request.py
--rw-rw-rw-   0        0        0     1400 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_request_py3.py
--rw-rw-rw-   0        0        0     1953 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_response.py
--rw-rw-rw-   0        0        0     1999 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_response_py3.py
--rw-rw-rw-   0        0        0     1638 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor.py
--rw-rw-rw-   0        0        0     1375 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_by_category_child.py
--rw-rw-rw-   0        0        0     1396 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_by_category_child_py3.py
--rw-rw-rw-   0        0        0     1038 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category.py
--rw-rw-rw-   0        0        0     1071 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_py3.py
--rw-rw-rw-   0        0        0     1317 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_response.py
--rw-rw-rw-   0        0        0     1344 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_response_py3.py
--rw-rw-rw-   0        0        0     1668 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_py3.py
--rw-rw-rw-   0        0        0     2528 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_version_history_response.py
--rw-rw-rw-   0        0        0     2548 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_version_history_response_py3.py
--rw-rw-rw-   0        0        0     2657 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factors_response.py
--rw-rw-rw-   0        0        0     2663 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factors_response_py3.py
--rw-rw-rw-   0        0        0     1196 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_gas.py
--rw-rw-rw-   0        0        0     1213 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_gas_py3.py
--rw-rw-rw-   0        0        0     1008 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_group_emissions.py
--rw-rw-rw-   0        0        0     1030 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_group_emissions_py3.py
--rw-rw-rw-   0        0        0     3413 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_performance_comparison.py
--rw-rw-rw-   0        0        0     3491 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_performance_comparison_py3.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope.py
--rw-rw-rw-   0        0        0     1492 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category.py
--rw-rw-rw-   0        0        0     1339 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_child.py
--rw-rw-rw-   0        0        0     1388 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_child_py3.py
--rw-rw-rw-   0        0        0     1533 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_py3.py
--rw-rw-rw-   0        0        0      886 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_py3.py
--rw-rw-rw-   0        0        0     1210 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_response.py
--rw-rw-rw-   0        0        0     1226 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_response_py3.py
--rw-rw-rw-   0        0        0     1280 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_request.py
--rw-rw-rw-   0        0        0     1291 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_request_py3.py
--rw-rw-rw-   0        0        0     1866 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_response.py
--rw-rw-rw-   0        0        0     1886 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_response_py3.py
--rw-rw-rw-   0        0        0     1505 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_settings.py
--rw-rw-rw-   0        0        0     1573 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_settings_py3.py
--rw-rw-rw-   0        0        0     1376 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_target_emissions.py
--rw-rw-rw-   0        0        0     1408 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_target_emissions_py3.py
--rw-rw-rw-   0        0        0     1133 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_type_child.py
--rw-rw-rw-   0        0        0     1157 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_type_child_py3.py
--rw-rw-rw-   0        0        0     1087 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_version.py
--rw-rw-rw-   0        0        0     1089 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_version_py3.py
--rw-rw-rw-   0        0        0     2361 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_yearly_emissions.py
--rw-rw-rw-   0        0        0     2434 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_yearly_emissions_py3.py
--rw-rw-rw-   0        0        0     1129 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child.py
--rw-rw-rw-   0        0        0     1148 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_py3.py
--rw-rw-rw-   0        0        0     1377 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_request.py
--rw-rw-rw-   0        0        0     1386 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_request_py3.py
--rw-rw-rw-   0        0        0     2276 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_request.py
--rw-rw-rw-   0        0        0     2290 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_request_py3.py
--rw-rw-rw-   0        0        0     1497 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_response.py
--rw-rw-rw-   0        0        0     1526 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_response_py3.py
--rw-rw-rw-   0        0        0     2018 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings.py
--rw-rw-rw-   0        0        0      897 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_class_permission.py
--rw-rw-rw-   0        0        0      904 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2067 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator.py
--rw-rw-rw-   0        0        0      762 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_class_permission.py
--rw-rw-rw-   0        0        0      772 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_class_permission_py3.py
--rw-rw-rw-   0        0        0     1935 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_py3.py
--rw-rw-rw-   0        0        0     3079 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_display_setting.py
--rw-rw-rw-   0        0        0     3167 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_display_setting_py3.py
--rw-rw-rw-   0        0        0     1043 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_member_request.py
--rw-rw-rw-   0        0        0     1059 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_member_request_py3.py
--rw-rw-rw-   0        0        0     4100 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_meter_group_response.py
--rw-rw-rw-   0        0        0     4227 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_meter_group_response_py3.py
--rw-rw-rw-   0        0        0     2017 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_member.py
--rw-rw-rw-   0        0        0     2032 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_member_py3.py
--rw-rw-rw-   0        0        0     3601 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_response.py
--rw-rw-rw-   0        0        0     3715 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_response_py3.py
--rw-rw-rw-   0        0        0     1868 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module.py
--rw-rw-rw-   0        0        0      747 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_class_permission.py
--rw-rw-rw-   0        0        0      755 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1918 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_py3.py
--rw-rw-rw-   0        0        0      735 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/guid_response.py
--rw-rw-rw-   0        0        0      748 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/guid_response_py3.py
--rw-rw-rw-   0        0        0      989 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hidden_request.py
--rw-rw-rw-   0        0        0      994 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hidden_request_py3.py
--rw-rw-rw-   0        0        0     3463 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers.py
--rw-rw-rw-   0        0        0     3023 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers2.py
--rw-rw-rw-   0        0        0     3134 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers2_py3.py
--rw-rw-rw-   0        0        0     3574 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers_py3.py
--rw-rw-rw-   0        0        0     3310 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places.py
--rw-rw-rw-   0        0        0     2940 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places2.py
--rw-rw-rw-   0        0        0     3020 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places2_py3.py
--rw-rw-rw-   0        0        0     3390 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places_py3.py
--rw-rw-rw-   0        0        0     1841 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data.py
--rw-rw-rw-   0        0        0     1853 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis.py
--rw-rw-rw-   0        0        0      732 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_class_permission.py
--rw-rw-rw-   0        0        0      740 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_class_permission_py3.py
--rw-rw-rw-   0        0        0     1903 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_py3.py
--rw-rw-rw-   0        0        0      720 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_class_permission.py
--rw-rw-rw-   0        0        0      730 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_class_permission_py3.py
--rw-rw-rw-   0        0        0     1893 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_py3.py
--rw-rw-rw-   0        0        0     1841 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup.py
--rw-rw-rw-   0        0        0      720 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_class_permission.py
--rw-rw-rw-   0        0        0      727 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_class_permission_py3.py
--rw-rw-rw-   0        0        0     1890 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_py3.py
--rw-rw-rw-   0        0        0     1381 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_response.py
--rw-rw-rw-   0        0        0     1389 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_response_py3.py
--rw-rw-rw-   0        0        0     1604 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_with_unit_response.py
--rw-rw-rw-   0        0        0     1609 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_with_unit_response_py3.py
--rw-rw-rw-   0        0        0     1533 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/latest_benchmark_value.py
--rw-rw-rw-   0        0        0     1568 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/latest_benchmark_value_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accounting_export.py
--rw-rw-rw-   0        0        0     1933 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accounting_export_py3.py
--rw-rw-rw-   0        0        0     1871 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accrual_bills.py
--rw-rw-rw-   0        0        0     1921 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accrual_bills_py3.py
--rw-rw-rw-   0        0        0     1868 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_chargebacks.py
--rw-rw-rw-   0        0        0     1918 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_chargebacks_py3.py
--rw-rw-rw-   0        0        0     1874 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_cost_avoidance.py
--rw-rw-rw-   0        0        0     1924 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_cost_avoidance_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_custom_benchmarks.py
--rw-rw-rw-   0        0        0     1933 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_custom_benchmarks_py3.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_ghg.py
--rw-rw-rw-   0        0        0     1894 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_ghg_py3.py
--rw-rw-rw-   0        0        0     1895 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_interval_data_analysis.py
--rw-rw-rw-   0        0        0     1945 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_interval_data_analysis_py3.py
--rw-rw-rw-   0        0        0     1877 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_designer.py
--rw-rw-rw-   0        0        0     1927 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_designer_py3.py
--rw-rw-rw-   0        0        0     1889 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_distribution.py
--rw-rw-rw-   0        0        0     1939 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_distribution_py3.py
--rw-rw-rw-   0        0        0     2873 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_features.py
--rw-rw-rw-   0        0        0     2952 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_features_py3.py
--rw-rw-rw-   0        0        0      820 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_request.py
--rw-rw-rw-   0        0        0      837 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_request_py3.py
--rw-rw-rw-   0        0        0     3076 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_response.py
--rw-rw-rw-   0        0        0     3128 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_response_py3.py
--rw-rw-rw-   0        0        0     1011 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_accrual_exclusion.py
--rw-rw-rw-   0        0        0     1017 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_accrual_exclusion_py3.py
--rw-rw-rw-   0        0        0      755 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_approve.py
--rw-rw-rw-   0        0        0      766 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_approve_py3.py
--rw-rw-rw-   0        0        0      976 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_custom.py
--rw-rw-rw-   0        0        0      984 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_custom_py3.py
--rw-rw-rw-   0        0        0      792 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_export_hold.py
--rw-rw-rw-   0        0        0      807 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_export_hold_py3.py
--rw-rw-rw-   0        0        0      773 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_reverse.py
--rw-rw-rw-   0        0        0      785 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_reverse_py3.py
--rw-rw-rw-   0        0        0      728 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_void.py
--rw-rw-rw-   0        0        0      736 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_void_py3.py
--rw-rw-rw-   0        0        0     2432 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_column_edit.py
--rw-rw-rw-   0        0        0     2423 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_column_edit_py3.py
--rw-rw-rw-   0        0        0     1381 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_copy.py
--rw-rw-rw-   0        0        0     1396 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_copy_py3.py
--rw-rw-rw-   0        0        0     1694 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create.py
--rw-rw-rw-   0        0        0     1708 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_py3.py
--rw-rw-rw-   0        0        0     1865 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_response.py
--rw-rw-rw-   0        0        0     1875 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_response_py3.py
--rw-rw-rw-   0        0        0     1444 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_edit.py
--rw-rw-rw-   0        0        0     1459 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_edit_py3.py
--rw-rw-rw-   0        0        0      707 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_ids.py
--rw-rw-rw-   0        0        0      708 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_ids_py3.py
--rw-rw-rw-   0        0        0     1597 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response.py
--rw-rw-rw-   0        0        0     2495 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_field.py
--rw-rw-rw-   0        0        0     2530 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_field_py3.py
--rw-rw-rw-   0        0        0      980 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_item.py
--rw-rw-rw-   0        0        0      979 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_item_py3.py
--rw-rw-rw-   0        0        0     1581 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_py3.py
--rw-rw-rw-   0        0        0     1128 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_type_child.py
--rw-rw-rw-   0        0        0     1162 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_type_child_py3.py
--rw-rw-rw-   0        0        0     1767 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_request.py
--rw-rw-rw-   0        0        0     1767 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_request_py3.py
--rw-rw-rw-   0        0        0      830 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_response.py
--rw-rw-rw-   0        0        0      829 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_response_py3.py
--rw-rw-rw-   0        0        0     2330 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manual_adjustment_request.py
--rw-rw-rw-   0        0        0     2349 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manual_adjustment_request_py3.py
--rw-rw-rw-   0        0        0     2000 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings.py
--rw-rw-rw-   0        0        0      879 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_class_permission.py
--rw-rw-rw-   0        0        0      886 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2049 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_py3.py
--rw-rw-rw-   0        0        0     3776 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_request.py
--rw-rw-rw-   0        0        0     3815 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_request_py3.py
--rw-rw-rw-   0        0        0     2985 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_response.py
--rw-rw-rw-   0        0        0     3028 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_response_py3.py
--rw-rw-rw-   0        0        0     2526 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_place_child.py
--rw-rw-rw-   0        0        0     2573 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_place_child_py3.py
--rw-rw-rw-   0        0        0     2254 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_widget_response.py
--rw-rw-rw-   0        0        0     2296 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_widget_response_py3.py
--rw-rw-rw-   0        0        0    10112 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/me.py
--rw-rw-rw-   0        0        0    10371 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_py3.py
--rw-rw-rw-   0        0        0     1303 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_request.py
--rw-rw-rw-   0        0        0     1309 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_request_py3.py
--rw-rw-rw-   0        0        0      943 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/message.py
--rw-rw-rw-   0        0        0      957 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/message_py3.py
--rw-rw-rw-   0        0        0     4342 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_account_child.py
--rw-rw-rw-   0        0        0     4425 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_account_child_py3.py
--rw-rw-rw-   0        0        0    13718 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_bill_response.py
--rw-rw-rw-   0        0        0    13849 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_bill_response_py3.py
--rw-rw-rw-   0        0        0     3166 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_calendarized_use_vs_weather_response.py
--rw-rw-rw-   0        0        0     3302 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_calendarized_use_vs_weather_response_py3.py
--rw-rw-rw-   0        0        0     1245 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cap_response.py
--rw-rw-rw-   0        0        0     1259 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cap_response_py3.py
--rw-rw-rw-   0        0        0     1680 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_request.py
--rw-rw-rw-   0        0        0     1715 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_request_py3.py
--rw-rw-rw-   0        0        0     2239 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_response.py
--rw-rw-rw-   0        0        0     2339 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_response_py3.py
--rw-rw-rw-   0        0        0     2713 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child.py
--rw-rw-rw-   0        0        0     3237 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_meter_import_id_and_route.py
--rw-rw-rw-   0        0        0     3287 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_meter_import_id_and_route_py3.py
--rw-rw-rw-   0        0        0     3059 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_and_serial_number.py
--rw-rw-rw-   0        0        0     3109 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_and_serial_number_py3.py
--rw-rw-rw-   0        0        0     3342 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_channel_latest_reading.py
--rw-rw-rw-   0        0        0     3387 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_channel_latest_reading_py3.py
--rw-rw-rw-   0        0        0     2764 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_py3.py
--rw-rw-rw-   0        0        0     3337 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_search.py
--rw-rw-rw-   0        0        0     3402 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_search_py3.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cost.py
--rw-rw-rw-   0        0        0     1234 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cost_py3.py
--rw-rw-rw-   0        0        0     5449 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_create.py
--rw-rw-rw-   0        0        0     5490 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_create_py3.py
--rw-rw-rw-   0        0        0     2572 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response.py
--rw-rw-rw-   0        0        0     2580 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_py3.py
--rw-rw-rw-   0        0        0     4151 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results.py
--rw-rw-rw-   0        0        0     4302 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     2566 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response.py
--rw-rw-rw-   0        0        0     2574 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_py3.py
--rw-rw-rw-   0        0        0     2295 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results.py
--rw-rw-rw-   0        0        0     2366 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     2517 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response.py
--rw-rw-rw-   0        0        0     2525 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_py3.py
--rw-rw-rw-   0        0        0     4398 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_results.py
--rw-rw-rw-   0        0        0     4566 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_results_py3.py
--rw-rw-rw-   0        0        0     2179 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response.py
--rw-rw-rw-   0        0        0     1680 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope.py
--rw-rw-rw-   0        0        0     1729 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope_py3.py
--rw-rw-rw-   0        0        0     1453 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type_py3.py
--rw-rw-rw-   0        0        0     2196 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1012 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_results.py
--rw-rw-rw-   0        0        0     1037 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     2324 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_py3.py
--rw-rw-rw-   0        0        0     3068 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_results.py
--rw-rw-rw-   0        0        0     3154 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     2318 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response.py
--rw-rw-rw-   0        0        0     2330 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1317 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_results.py
--rw-rw-rw-   0        0        0     1339 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     2463 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response.py
--rw-rw-rw-   0        0        0     2462 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_py3.py
--rw-rw-rw-   0        0        0     3409 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_results.py
--rw-rw-rw-   0        0        0     3503 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     5516 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response.py
--rw-rw-rw-   0        0        0     5679 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_py3.py
--rw-rw-rw-   0        0        0     2883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_results.py
--rw-rw-rw-   0        0        0     2968 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     6184 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_edit.py
--rw-rw-rw-   0        0        0     6219 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_edit_py3.py
--rw-rw-rw-   0        0        0     1311 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_category_child.py
--rw-rw-rw-   0        0        0     1371 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_category_child_py3.py
--rw-rw-rw-   0        0        0     1718 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_child.py
--rw-rw-rw-   0        0        0     1770 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_child_py3.py
--rw-rw-rw-   0        0        0     2660 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_child.py
--rw-rw-rw-   0        0        0     2724 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_child_py3.py
--rw-rw-rw-   0        0        0     2973 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_child.py
--rw-rw-rw-   0        0        0     3034 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_child_py3.py
--rw-rw-rw-   0        0        0     4066 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_response.py
--rw-rw-rw-   0        0        0     4161 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_response_py3.py
--rw-rw-rw-   0        0        0     3599 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_child.py
--rw-rw-rw-   0        0        0     3669 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_child_py3.py
--rw-rw-rw-   0        0        0     5914 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_response.py
--rw-rw-rw-   0        0        0     6070 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_response_py3.py
--rw-rw-rw-   0        0        0     1169 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member.py
--rw-rw-rw-   0        0        0     3470 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_child.py
--rw-rw-rw-   0        0        0     3518 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_child_py3.py
--rw-rw-rw-   0        0        0     1196 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_py3.py
--rw-rw-rw-   0        0        0     2959 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_request.py
--rw-rw-rw-   0        0        0     3012 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_request_py3.py
--rw-rw-rw-   0        0        0     2277 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_response.py
--rw-rw-rw-   0        0        0     2335 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_response_py3.py
--rw-rw-rw-   0        0        0     2020 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_rate_response.py
--rw-rw-rw-   0        0        0     2005 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_rate_response_py3.py
--rw-rw-rw-   0        0        0     7316 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_response.py
--rw-rw-rw-   0        0        0     7381 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_response_py3.py
--rw-rw-rw-   0        0        0     1997 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings.py
--rw-rw-rw-   0        0        0      876 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_class_permission.py
--rw-rw-rw-   0        0        0      883 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2046 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_py3.py
--rw-rw-rw-   0        0        0     1626 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_search_request.py
--rw-rw-rw-   0        0        0     1637 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_search_request_py3.py
--rw-rw-rw-   0        0        0     1149 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_child.py
--rw-rw-rw-   0        0        0     1186 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_child_py3.py
--rw-rw-rw-   0        0        0     1531 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_request.py
--rw-rw-rw-   0        0        0     1558 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_request_py3.py
--rw-rw-rw-   0        0        0     1406 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_response.py
--rw-rw-rw-   0        0        0     1430 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_response_py3.py
--rw-rw-rw-   0        0        0     1839 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_template_response.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_template_response_py3.py
--rw-rw-rw-   0        0        0     1107 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_type_child.py
--rw-rw-rw-   0        0        0     1137 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_type_child_py3.py
--rw-rw-rw-   0        0        0     1296 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_udf_response.py
--rw-rw-rw-   0        0        0     1302 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_udf_response_py3.py
--rw-rw-rw-   0        0        0     2231 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters.py
--rw-rw-rw-   0        0        0     1110 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_class_permission.py
--rw-rw-rw-   0        0        0     1113 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_class_permission_py3.py
--rw-rw-rw-   0        0        0     2276 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_py3.py
--rw-rw-rw-   0        0        0     1839 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/missing_bill_widget.py
--rw-rw-rw-   0        0        0     1858 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/missing_bill_widget_py3.py
--rw-rw-rw-   0        0        0     1706 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/monthly_cap_trend.py
--rw-rw-rw-   0        0        0     1747 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/monthly_cap_trend_py3.py
--rw-rw-rw-   0        0        0     1039 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/most_recent_aggregate.py
--rw-rw-rw-   0        0        0     1061 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/most_recent_aggregate_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors.py
--rw-rw-rw-   0        0        0      762 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_class_permission.py
--rw-rw-rw-   0        0        0      772 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_class_permission_py3.py
--rw-rw-rw-   0        0        0     1935 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_py3.py
--rw-rw-rw-   0        0        0     1137 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_bills_destination.py
--rw-rw-rw-   0        0        0     1141 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_bills_destination_py3.py
--rw-rw-rw-   0        0        0     1337 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_create_meter.py
--rw-rw-rw-   0        0        0     1356 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_create_meter_py3.py
--rw-rw-rw-   0        0        0     1856 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills.py
--rw-rw-rw-   0        0        0      735 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_class_permission.py
--rw-rw-rw-   0        0        0      745 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_class_permission_py3.py
--rw-rw-rw-   0        0        0     1908 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_py3.py
--rw-rw-rw-   0        0        0     1156 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/named_period.py
--rw-rw-rw-   0        0        0     1168 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/named_period_py3.py
--rw-rw-rw-   0        0        0     2000 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings.py
--rw-rw-rw-   0        0        0      879 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_class_permission.py
--rw-rw-rw-   0        0        0      886 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2049 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_py3.py
--rw-rw-rw-   0        0        0     1177 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_action_button_response.py
--rw-rw-rw-   0        0        0     1191 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_action_button_response_py3.py
--rw-rw-rw-   0        0        0     1450 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_badge_response.py
--rw-rw-rw-   0        0        0     1492 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_badge_response_py3.py
--rw-rw-rw-   0        0        0     1480 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_category.py
--rw-rw-rw-   0        0        0     1550 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_category_py3.py
--rw-rw-rw-   0        0        0     2803 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_details_response.py
--rw-rw-rw-   0        0        0     2826 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_details_response_py3.py
--rw-rw-rw-   0        0        0     2073 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_response.py
--rw-rw-rw-   0        0        0     2098 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_response_py3.py
--rw-rw-rw-   0        0        0     1848 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_request.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_request_py3.py
--rw-rw-rw-   0        0        0     1513 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_response.py
--rw-rw-rw-   0        0        0     1567 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_response_py3.py
--rw-rw-rw-   0        0        0     1328 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_settings_response.py
--rw-rw-rw-   0        0        0     1374 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_settings_response_py3.py
--rw-rw-rw-   0        0        0     1711 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_system_settings_request.py
--rw-rw-rw-   0        0        0     1752 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_system_settings_request_py3.py
--rw-rw-rw-   0        0        0     1671 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_type.py
--rw-rw-rw-   0        0        0     1737 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_type_py3.py
--rw-rw-rw-   0        0        0     1643 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_update_request.py
--rw-rw-rw-   0        0        0     1650 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_update_request_py3.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_method_child.py
--rw-rw-rw-   0        0        0     1477 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_method_child_py3.py
--rw-rw-rw-   0        0        0     1302 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_rule.py
--rw-rw-rw-   0        0        0     1350 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_rule_py3.py
--rw-rw-rw-   0        0        0     2143 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type.py
--rw-rw-rw-   0        0        0     1964 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child.py
--rw-rw-rw-   0        0        0     1329 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_base.py
--rw-rw-rw-   0        0        0     1377 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_base_py3.py
--rw-rw-rw-   0        0        0     2010 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_py3.py
--rw-rw-rw-   0        0        0     2188 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_py3.py
--rw-rw-rw-   0        0        0     1719 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_object_result.py
--rw-rw-rw-   0        0        0     1727 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_object_result_py3.py
--rw-rw-rw-   0        0        0      690 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_result.py
--rw-rw-rw-   0        0        0      704 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_result_py3.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category.py
--rw-rw-rw-   0        0        0     1182 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_py3.py
--rw-rw-rw-   0        0        0      869 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_request.py
--rw-rw-rw-   0        0        0      899 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_request_py3.py
--rw-rw-rw-   0        0        0     3459 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_request.py
--rw-rw-rw-   0        0        0     3501 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_request_py3.py
--rw-rw-rw-   0        0        0     3759 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_response.py
--rw-rw-rw-   0        0        0     3817 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_response_py3.py
--rw-rw-rw-   0        0        0     1566 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/outlier_severity_child.py
--rw-rw-rw-   0        0        0     1598 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/outlier_severity_child_py3.py
--rw-rw-rw-   0        0        0     1485 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_comparison.py
--rw-rw-rw-   0        0        0     1510 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_comparison_py3.py
--rw-rw-rw-   0        0        0      951 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range.py
--rw-rw-rw-   0        0        0     1110 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison.py
--rw-rw-rw-   0        0        0     1818 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_detailed.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_detailed_py3.py
--rw-rw-rw-   0        0        0     1136 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_py3.py
--rw-rw-rw-   0        0        0      968 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_py3.py
--rw-rw-rw-   0        0        0     1103 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_value.py
--rw-rw-rw-   0        0        0     1118 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_value_py3.py
--rw-rw-rw-   0        0        0    23430 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions.py
--rw-rw-rw-   0        0        0    24140 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_py3.py
--rw-rw-rw-   0        0        0    22391 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_request.py
--rw-rw-rw-   0        0        0    22943 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_request_py3.py
--rw-rw-rw-   0        0        0     1680 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_request.py
--rw-rw-rw-   0        0        0     1715 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_request_py3.py
--rw-rw-rw-   0        0        0     2239 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_response.py
--rw-rw-rw-   0        0        0     2339 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_response_py3.py
--rw-rw-rw-   0        0        0     1274 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child.py
--rw-rw-rw-   0        0        0     1286 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_py3.py
--rw-rw-rw-   0        0        0     1587 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_with_floor_area.py
--rw-rw-rw-   0        0        0     1604 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_with_floor_area_py3.py
--rw-rw-rw-   0        0        0     1852 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_cost.py
--rw-rw-rw-   0        0        0     1876 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_cost_py3.py
--rw-rw-rw-   0        0        0     3811 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_create.py
--rw-rw-rw-   0        0        0     3836 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_create_py3.py
--rw-rw-rw-   0        0        0     2969 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response.py
--rw-rw-rw-   0        0        0     2594 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2622 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     3916 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results.py
--rw-rw-rw-   0        0        0     4059 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2971 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_py3.py
--rw-rw-rw-   0        0        0     2736 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results.py
--rw-rw-rw-   0        0        0     2822 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     2801 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response.py
--rw-rw-rw-   0        0        0     2634 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2662 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     2322 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     2393 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2804 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1383 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results.py
--rw-rw-rw-   0        0        0     1412 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     2034 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison.py
--rw-rw-rw-   0        0        0     2076 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison_py3.py
--rw-rw-rw-   0        0        0     2007 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_comparison_response.py
--rw-rw-rw-   0        0        0     2021 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_comparison_response_py3.py
--rw-rw-rw-   0        0        0     2530 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity.py
--rw-rw-rw-   0        0        0     1629 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity.py
--rw-rw-rw-   0        0        0     1658 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity_py3.py
--rw-rw-rw-   0        0        0     1598 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project.py
--rw-rw-rw-   0        0        0     1651 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project_py3.py
--rw-rw-rw-   0        0        0     2570 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_py3.py
--rw-rw-rw-   0        0        0     2583 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response.py
--rw-rw-rw-   0        0        0     1808 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity.py
--rw-rw-rw-   0        0        0     1833 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity_py3.py
--rw-rw-rw-   0        0        0     1801 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope.py
--rw-rw-rw-   0        0        0     1826 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope_py3.py
--rw-rw-rw-   0        0        0     1777 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type.py
--rw-rw-rw-   0        0        0     1799 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type_py3.py
--rw-rw-rw-   0        0        0     2599 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_py3.py
--rw-rw-rw-   0        0        0     1860 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_results.py
--rw-rw-rw-   0        0        0     1912 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     1277 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison.py
--rw-rw-rw-   0        0        0     1289 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison_py3.py
--rw-rw-rw-   0        0        0     2246 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response.py
--rw-rw-rw-   0        0        0     1971 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope.py
--rw-rw-rw-   0        0        0     2016 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope_py3.py
--rw-rw-rw-   0        0        0     1769 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type.py
--rw-rw-rw-   0        0        0     1791 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type_py3.py
--rw-rw-rw-   0        0        0     2264 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1012 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_results.py
--rw-rw-rw-   0        0        0     1037 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1690 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison.py
--rw-rw-rw-   0        0        0     1748 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison_py3.py
--rw-rw-rw-   0        0        0     1362 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly.py
--rw-rw-rw-   0        0        0     2499 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results.py
--rw-rw-rw-   0        0        0     2563 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results_py3.py
--rw-rw-rw-   0        0        0     1374 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_py3.py
--rw-rw-rw-   0        0        0     2504 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response.py
--rw-rw-rw-   0        0        0     2384 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2416 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     2448 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results.py
--rw-rw-rw-   0        0        0     2512 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2511 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_py3.py
--rw-rw-rw-   0        0        0     1784 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_results.py
--rw-rw-rw-   0        0        0     1822 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     1299 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly.py
--rw-rw-rw-   0        0        0     1311 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_py3.py
--rw-rw-rw-   0        0        0     1808 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results.py
--rw-rw-rw-   0        0        0     1846 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results_py3.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2145 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1143 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1158 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2516 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_py3.py
--rw-rw-rw-   0        0        0      929 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_results.py
--rw-rw-rw-   0        0        0      940 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1510 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison.py
--rw-rw-rw-   0        0        0     1540 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison_py3.py
--rw-rw-rw-   0        0        0     2374 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response.py
--rw-rw-rw-   0        0        0     2005 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2366 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results.py
--rw-rw-rw-   0        0        0     2436 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2024 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     2373 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_py3.py
--rw-rw-rw-   0        0        0     2065 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_results.py
--rw-rw-rw-   0        0        0     2123 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_results_py3.py
--rw-rw-rw-   0        0        0     4245 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response.py
--rw-rw-rw-   0        0        0     4797 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2948 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results.py
--rw-rw-rw-   0        0        0     3033 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results_py3.py
--rw-rw-rw-   0        0        0     4975 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     4350 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_py3.py
--rw-rw-rw-   0        0        0     2170 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_results.py
--rw-rw-rw-   0        0        0     2229 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1249 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly.py
--rw-rw-rw-   0        0        0     1261 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_py3.py
--rw-rw-rw-   0        0        0     1778 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_results.py
--rw-rw-rw-   0        0        0     1816 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_results_py3.py
--rw-rw-rw-   0        0        0     4085 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_edit.py
--rw-rw-rw-   0        0        0     4110 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_edit_py3.py
--rw-rw-rw-   0        0        0     1311 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_category_child.py
--rw-rw-rw-   0        0        0     1371 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_category_child_py3.py
--rw-rw-rw-   0        0        0     1718 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_child.py
--rw-rw-rw-   0        0        0     1770 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_child_py3.py
--rw-rw-rw-   0        0        0     2600 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_child.py
--rw-rw-rw-   0        0        0     2641 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_child_py3.py
--rw-rw-rw-   0        0        0     6503 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_response.py
--rw-rw-rw-   0        0        0     6630 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_response_py3.py
--rw-rw-rw-   0        0        0     2199 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_child.py
--rw-rw-rw-   0        0        0     2231 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_child_py3.py
--rw-rw-rw-   0        0        0     5496 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_response.py
--rw-rw-rw-   0        0        0     5591 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_response_py3.py
--rw-rw-rw-   0        0        0     1432 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_child.py
--rw-rw-rw-   0        0        0     1462 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_child_py3.py
--rw-rw-rw-   0        0        0     1818 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_child.py
--rw-rw-rw-   0        0        0     1857 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_child_py3.py
--rw-rw-rw-   0        0        0     5090 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_response.py
--rw-rw-rw-   0        0        0     5256 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_response_py3.py
--rw-rw-rw-   0        0        0     1169 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_member.py
--rw-rw-rw-   0        0        0     1196 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_member_py3.py
--rw-rw-rw-   0        0        0     2959 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_request.py
--rw-rw-rw-   0        0        0     3012 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_request_py3.py
--rw-rw-rw-   0        0        0     2277 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_response.py
--rw-rw-rw-   0        0        0     2335 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_response_py3.py
--rw-rw-rw-   0        0        0     1056 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_info.py
--rw-rw-rw-   0        0        0     1071 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_info_py3.py
--rw-rw-rw-   0        0        0     5861 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_response.py
--rw-rw-rw-   0        0        0     5838 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_response_py3.py
--rw-rw-rw-   0        0        0     2127 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_child.py
--rw-rw-rw-   0        0        0     2135 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_child_py3.py
--rw-rw-rw-   0        0        0     2196 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_create.py
--rw-rw-rw-   0        0        0     2192 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_create_py3.py
--rw-rw-rw-   0        0        0     1278 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_submission_type_request.py
--rw-rw-rw-   0        0        0     1292 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_submission_type_request_py3.py
--rw-rw-rw-   0        0        0     1030 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_request.py
--rw-rw-rw-   0        0        0     1043 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_request_py3.py
--rw-rw-rw-   0        0        0     1382 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_response.py
--rw-rw-rw-   0        0        0     1414 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_response_py3.py
--rw-rw-rw-   0        0        0     1296 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_udf_response.py
--rw-rw-rw-   0        0        0     1302 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_udf_response_py3.py
--rw-rw-rw-   0        0        0     1034 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/pm_commodity_child.py
--rw-rw-rw-   0        0        0     1057 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/pm_commodity_child_py3.py
--rw-rw-rw-   0        0        0     1518 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response.py
--rw-rw-rw-   0        0        0     1526 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_py3.py
--rw-rw-rw-   0        0        0     1796 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_weather_station.py
--rw-rw-rw-   0        0        0     1827 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_weather_station_py3.py
--rw-rw-rw-   0        0        0     6804 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference.py
--rw-rw-rw-   0        0        0     7093 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_py3.py
--rw-rw-rw-   0        0        0     7718 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_request.py
--rw-rw-rw-   0        0        0     7996 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_request_py3.py
--rw-rw-rw-   0        0        0     1128 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_child.py
--rw-rw-rw-   0        0        0     1161 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_child_py3.py
--rw-rw-rw-   0        0        0     1985 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_create.py
--rw-rw-rw-   0        0        0     2005 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_create_py3.py
--rw-rw-rw-   0        0        0     1337 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_response.py
--rw-rw-rw-   0        0        0     1378 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_response_py3.py
--rw-rw-rw-   0        0        0     1100 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/project_manager_response.py
--rw-rw-rw-   0        0        0     1140 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/project_manager_response_py3.py
--rw-rw-rw-   0        0        0     1871 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps.py
--rw-rw-rw-   0        0        0      750 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_class_permission.py
--rw-rw-rw-   0        0        0      760 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_class_permission_py3.py
--rw-rw-rw-   0        0        0     1923 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_py3.py
--rw-rw-rw-   0        0        0     1365 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_filter.py
--rw-rw-rw-   0        0        0     1357 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_filter_py3.py
--rw-rw-rw-   0        0        0     1574 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_report.py
--rw-rw-rw-   0        0        0     1581 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_report_py3.py
--rw-rw-rw-   0        0        0      799 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child.py
--rw-rw-rw-   0        0        0      805 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_py3.py
--rw-rw-rw-   0        0        0     1027 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_response.py
--rw-rw-rw-   0        0        0     1029 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_response_py3.py
--rw-rw-rw-   0        0        0     1788 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_create.py
--rw-rw-rw-   0        0        0     1781 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_create_py3.py
--rw-rw-rw-   0        0        0     2114 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response.py
--rw-rw-rw-   0        0        0     1956 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     1975 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1804 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1851 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2104 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1349 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_results.py
--rw-rw-rw-   0        0        0     1378 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1204 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_edit.py
--rw-rw-rw-   0        0        0     1207 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_edit_py3.py
--rw-rw-rw-   0        0        0     1530 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_response.py
--rw-rw-rw-   0        0        0     1516 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_response_py3.py
--rw-rw-rw-   0        0        0     2120 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules.py
--rw-rw-rw-   0        0        0      999 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_class_permission.py
--rw-rw-rw-   0        0        0     1005 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_class_permission_py3.py
--rw-rw-rw-   0        0        0     2168 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_py3.py
--rw-rw-rw-   0        0        0     3957 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_request.py
--rw-rw-rw-   0        0        0     3985 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_request_py3.py
--rw-rw-rw-   0        0        0     3982 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_response.py
--rw-rw-rw-   0        0        0     3982 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_response_py3.py
--rw-rw-rw-   0        0        0     1744 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading.py
--rw-rw-rw-   0        0        0     1464 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_child_base.py
--rw-rw-rw-   0        0        0     1469 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_child_base_py3.py
--rw-rw-rw-   0        0        0     4330 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_create.py
--rw-rw-rw-   0        0        0     4382 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_create_py3.py
--rw-rw-rw-   0        0        0     1627 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_delete.py
--rw-rw-rw-   0        0        0     1627 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_delete_py3.py
--rw-rw-rw-   0        0        0     6736 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile.py
--rw-rw-rw-   0        0        0     1932 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_column.py
--rw-rw-rw-   0        0        0     1952 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_column_py3.py
--rw-rw-rw-   0        0        0     6876 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_py3.py
--rw-rw-rw-   0        0        0     7173 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_request.py
--rw-rw-rw-   0        0        0     7312 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_request_py3.py
--rw-rw-rw-   0        0        0     5583 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_response.py
--rw-rw-rw-   0        0        0     5733 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_response_py3.py
--rw-rw-rw-   0        0        0     1829 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_request.py
--rw-rw-rw-   0        0        0     1852 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_request_py3.py
--rw-rw-rw-   0        0        0     1733 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_py3.py
--rw-rw-rw-   0        0        0     1405 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_response.py
--rw-rw-rw-   0        0        0     1446 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_response_py3.py
--rw-rw-rw-   0        0        0     1260 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings.py
--rw-rw-rw-   0        0        0     2101 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_observation.py
--rw-rw-rw-   0        0        0     2109 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_observation_py3.py
--rw-rw-rw-   0        0        0     1255 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_py3.py
--rw-rw-rw-   0        0        0     1447 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/related_report_response.py
--rw-rw-rw-   0        0        0     1472 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/related_report_response_py3.py
--rw-rw-rw-   0        0        0     1862 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator.py
--rw-rw-rw-   0        0        0      741 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_class_permission.py
--rw-rw-rw-   0        0        0      751 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_class_permission_py3.py
--rw-rw-rw-   0        0        0     1914 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_py3.py
--rw-rw-rw-   0        0        0     1212 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_category_child.py
--rw-rw-rw-   0        0        0     1257 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_category_child_py3.py
--rw-rw-rw-   0        0        0     2986 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_child.py
--rw-rw-rw-   0        0        0     3005 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_child_py3.py
--rw-rw-rw-   0        0        0     1828 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_create.py
--rw-rw-rw-   0        0        0     1840 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_create_py3.py
--rw-rw-rw-   0        0        0     1580 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_child.py
--rw-rw-rw-   0        0        0     1626 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_child_py3.py
--rw-rw-rw-   0        0        0     6134 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_create_request.py
--rw-rw-rw-   0        0        0     6203 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_create_request_py3.py
--rw-rw-rw-   0        0        0     3503 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_details_response.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_details_response_py3.py
--rw-rw-rw-   0        0        0     5911 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_edit_request.py
--rw-rw-rw-   0        0        0     5970 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_edit_request_py3.py
--rw-rw-rw-   0        0        0     2873 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_email_settings.py
--rw-rw-rw-   0        0        0     2923 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_email_settings_py3.py
--rw-rw-rw-   0        0        0     1384 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_details_response.py
--rw-rw-rw-   0        0        0     1396 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_details_response_py3.py
--rw-rw-rw-   0        0        0     3152 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_email_settings.py
--rw-rw-rw-   0        0        0     3209 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_email_settings_py3.py
--rw-rw-rw-   0        0        0     1089 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_report_settings.py
--rw-rw-rw-   0        0        0     1099 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_report_settings_py3.py
--rw-rw-rw-   0        0        0     2261 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_response.py
--rw-rw-rw-   0        0        0     2298 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_response_py3.py
--rw-rw-rw-   0        0        0     1820 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_edit.py
--rw-rw-rw-   0        0        0     1832 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_edit_py3.py
--rw-rw-rw-   0        0        0     1173 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_child_response.py
--rw-rw-rw-   0        0        0     1209 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_child_response_py3.py
--rw-rw-rw-   0        0        0     1134 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_request.py
--rw-rw-rw-   0        0        0     1160 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_request_py3.py
--rw-rw-rw-   0        0        0     1352 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_response.py
--rw-rw-rw-   0        0        0     1382 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_response_py3.py
--rw-rw-rw-   0        0        0     1841 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups.py
--rw-rw-rw-   0        0        0      720 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_class_permission.py
--rw-rw-rw-   0        0        0      730 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_class_permission_py3.py
--rw-rw-rw-   0        0        0     1893 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_py3.py
--rw-rw-rw-   0        0        0     2949 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_child.py
--rw-rw-rw-   0        0        0     2997 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_child_py3.py
--rw-rw-rw-   0        0        0     1519 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_day_indicator_child.py
--rw-rw-rw-   0        0        0     1551 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_day_indicator_child_py3.py
--rw-rw-rw-   0        0        0     3749 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_request.py
--rw-rw-rw-   0        0        0     3794 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_request_py3.py
--rw-rw-rw-   0        0        0     1350 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_child.py
--rw-rw-rw-   0        0        0     1419 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_child_py3.py
--rw-rw-rw-   0        0        0     1669 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_response.py
--rw-rw-rw-   0        0        0     1739 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_response_py3.py
--rw-rw-rw-   0        0        0     1189 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_type.py
--rw-rw-rw-   0        0        0     1222 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_type_py3.py
--rw-rw-rw-   0        0        0     1808 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports.py
--rw-rw-rw-   0        0        0      687 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_class_permission.py
--rw-rw-rw-   0        0        0      694 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_class_permission_py3.py
--rw-rw-rw-   0        0        0     1832 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module.py
--rw-rw-rw-   0        0        0      711 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_class_permission.py
--rw-rw-rw-   0        0        0      719 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1882 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_py3.py
--rw-rw-rw-   0        0        0     1857 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_py3.py
--rw-rw-rw-   0        0        0     3920 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/required_address_child.py
--rw-rw-rw-   0        0        0     3924 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/required_address_child_py3.py
--rw-rw-rw-   0        0        0     1859 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords.py
--rw-rw-rw-   0        0        0      738 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_class_permission.py
--rw-rw-rw-   0        0        0      748 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_class_permission_py3.py
--rw-rw-rw-   0        0        0     1911 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_py3.py
--rw-rw-rw-   0        0        0     1142 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reviewed.py
--rw-rw-rw-   0        0        0     1152 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/reviewed_py3.py
--rw-rw-rw-   0        0        0     1820 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles.py
--rw-rw-rw-   0        0        0      699 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_class_permission.py
--rw-rw-rw-   0        0        0      709 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_class_permission_py3.py
--rw-rw-rw-   0        0        0     1872 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_py3.py
--rw-rw-rw-   0        0        0      992 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_detail.py
--rw-rw-rw-   0        0        0      993 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_detail_py3.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_response.py
--rw-rw-rw-   0        0        0     1482 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_response_py3.py
--rw-rw-rw-   0        0        0     1323 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update.py
--rw-rw-rw-   0        0        0     1186 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_common_unit.py
--rw-rw-rw-   0        0        0     1214 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_common_unit_py3.py
--rw-rw-rw-   0        0        0     1348 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_py3.py
--rw-rw-rw-   0        0        0     1059 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_child.py
--rw-rw-rw-   0        0        0     1074 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_child_py3.py
--rw-rw-rw-   0        0        0     1612 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_details_response.py
--rw-rw-rw-   0        0        0     1628 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_details_response_py3.py
--rw-rw-rw-   0        0        0     1133 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter.py
--rw-rw-rw-   0        0        0     1452 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_channel_latest_reading_response.py
--rw-rw-rw-   0        0        0     1460 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_channel_latest_reading_response_py3.py
--rw-rw-rw-   0        0        0     1144 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_py3.py
--rw-rw-rw-   0        0        0     2024 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_request.py
--rw-rw-rw-   0        0        0     2025 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_request_py3.py
--rw-rw-rw-   0        0        0     1312 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_response.py
--rw-rw-rw-   0        0        0     1335 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_response_py3.py
--rw-rw-rw-   0        0        0     1991 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments.py
--rw-rw-rw-   0        0        0      870 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_class_permission.py
--rw-rw-rw-   0        0        0      877 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_class_permission_py3.py
--rw-rw-rw-   0        0        0     2040 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_py3.py
--rw-rw-rw-   0        0        0     5456 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_daily_data.py
--rw-rw-rw-   0        0        0     5676 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_daily_data_py3.py
--rw-rw-rw-   0        0        0     1826 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine.py
--rw-rw-rw-   0        0        0      705 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_class_permission.py
--rw-rw-rw-   0        0        0      712 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_class_permission_py3.py
--rw-rw-rw-   0        0        0     1875 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_py3.py
--rw-rw-rw-   0        0        0     1757 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_log.py
--rw-rw-rw-   0        0        0     1787 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_log_py3.py
--rw-rw-rw-   0        0        0     3255 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_daily_response.py
--rw-rw-rw-   0        0        0     3286 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_daily_response_py3.py
--rw-rw-rw-   0        0        0     8969 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_response.py
--rw-rw-rw-   0        0        0     9208 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_response_py3.py
--rw-rw-rw-   0        0        0      779 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child.py
--rw-rw-rw-   0        0        0      783 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_py3.py
--rw-rw-rw-   0        0        0     3944 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_search_account_child.py
--rw-rw-rw-   0        0        0     3993 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_search_account_child_py3.py
--rw-rw-rw-   0        0        0     3885 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_meter_bill_entry.py
--rw-rw-rw-   0        0        0     3949 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_meter_bill_entry_py3.py
--rw-rw-rw-   0        0        0      790 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child.py
--rw-rw-rw-   0        0        0      794 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_py3.py
--rw-rw-rw-   0        0        0     2113 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_search_cost_center.py
--rw-rw-rw-   0        0        0     2134 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_search_cost_center_py3.py
--rw-rw-rw-   0        0        0      765 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child.py
--rw-rw-rw-   0        0        0      769 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_py3.py
--rw-rw-rw-   0        0        0     5794 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_search_meter_child.py
--rw-rw-rw-   0        0        0     5842 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_search_meter_child_py3.py
--rw-rw-rw-   0        0        0     1310 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_parent_place_child.py
--rw-rw-rw-   0        0        0     1322 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_parent_place_child_py3.py
--rw-rw-rw-   0        0        0      765 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child.py
--rw-rw-rw-   0        0        0      769 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_py3.py
--rw-rw-rw-   0        0        0     2374 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_search_place_child.py
--rw-rw-rw-   0        0        0     2368 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_search_place_child_py3.py
--rw-rw-rw-   0        0        0      731 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_group.py
--rw-rw-rw-   0        0        0      735 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_group_py3.py
--rw-rw-rw-   0        0        0     1762 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_response.py
--rw-rw-rw-   0        0        0     1752 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_response_py3.py
--rw-rw-rw-   0        0        0     2077 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_data_access_release_request.py
--rw-rw-rw-   0        0        0     2068 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_data_access_release_request_py3.py
--rw-rw-rw-   0        0        0     1856 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications.py
--rw-rw-rw-   0        0        0      735 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_class_permission.py
--rw-rw-rw-   0        0        0      745 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_class_permission_py3.py
--rw-rw-rw-   0        0        0     1908 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_py3.py
--rw-rw-rw-   0        0        0     3655 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/setup.py
--rw-rw-rw-   0        0        0     3634 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/setup_py3.py
--rw-rw-rw-   0        0        0     2022 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_request.py
--rw-rw-rw-   0        0        0     2041 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_request_py3.py
--rw-rw-rw-   0        0        0     1510 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_response.py
--rw-rw-rw-   0        0        0     1538 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_response_py3.py
--rw-rw-rw-   0        0        0     2114 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists.py
--rw-rw-rw-   0        0        0      993 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_class_permission.py
--rw-rw-rw-   0        0        0      997 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_class_permission_py3.py
--rw-rw-rw-   0        0        0     2160 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_py3.py
--rw-rw-rw-   0        0        0     2135 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps.py
--rw-rw-rw-   0        0        0     1014 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_class_permission.py
--rw-rw-rw-   0        0        0     1018 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_class_permission_py3.py
--rw-rw-rw-   0        0        0     2181 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_py3.py
--rw-rw-rw-   0        0        0     2108 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports.py
--rw-rw-rw-   0        0        0      987 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_class_permission.py
--rw-rw-rw-   0        0        0      991 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_class_permission_py3.py
--rw-rw-rw-   0        0        0     2154 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_py3.py
--rw-rw-rw-   0        0        0      672 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_boolean.py
--rw-rw-rw-   0        0        0      681 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_boolean_py3.py
--rw-rw-rw-   0        0        0      670 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_value.py
--rw-rw-rw-   0        0        0      673 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_value_py3.py
--rw-rw-rw-   0        0        0     3821 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_create.py
--rw-rw-rw-   0        0        0     3860 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_create_py3.py
--rw-rw-rw-   0        0        0     3493 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_edit.py
--rw-rw-rw-   0        0        0     3536 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_edit_py3.py
--rw-rw-rw-   0        0        0     1704 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_method.py
--rw-rw-rw-   0        0        0     1737 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_method_py3.py
--rw-rw-rw-   0        0        0     3137 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_response.py
--rw-rw-rw-   0        0        0     3186 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_response_py3.py
--rw-rw-rw-   0        0        0     1452 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_type.py
--rw-rw-rw-   0        0        0     1521 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_type_py3.py
--rw-rw-rw-   0        0        0     3447 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_report_response.py
--rw-rw-rw-   0        0        0     3488 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_report_response_py3.py
--rw-rw-rw-   0        0        0     2394 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_widget_response.py
--rw-rw-rw-   0        0        0     2412 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_widget_response_py3.py
--rw-rw-rw-   0        0        0     2212 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request.py
--rw-rw-rw-   0        0        0     2225 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request_py3.py
--rw-rw-rw-   0        0        0     2242 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response.py
--rw-rw-rw-   0        0        0     2270 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response_py3.py
--rw-rw-rw-   0        0        0     2073 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statistics_response.py
--rw-rw-rw-   0        0        0     2090 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/statistics_response_py3.py
--rw-rw-rw-   0        0        0     1068 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/submission_type_response.py
--rw-rw-rw-   0        0        0     1101 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/submission_type_response_py3.py
--rw-rw-rw-   0        0        0     1394 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_request.py
--rw-rw-rw-   0        0        0     1421 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_request_py3.py
--rw-rw-rw-   0        0        0     1275 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_response.py
--rw-rw-rw-   0        0        0     1296 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_response_py3.py
--rw-rw-rw-   0        0        0     1317 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_request.py
--rw-rw-rw-   0        0        0     1334 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_request_py3.py
--rw-rw-rw-   0        0        0     1203 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_response.py
--rw-rw-rw-   0        0        0     1214 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_response_py3.py
--rw-rw-rw-   0        0        0     5610 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_request.py
--rw-rw-rw-   0        0        0     5780 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_request_py3.py
--rw-rw-rw-   0        0        0     3774 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_response.py
--rw-rw-rw-   0        0        0     3914 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_response_py3.py
--rw-rw-rw-   0        0        0      960 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_child.py
--rw-rw-rw-   0        0        0      981 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_child_py3.py
--rw-rw-rw-   0        0        0     2303 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_response.py
--rw-rw-rw-   0        0        0     2352 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_response_py3.py
--rw-rw-rw-   0        0        0     2088 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_with_hidden_request.py
--rw-rw-rw-   0        0        0     2102 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_with_hidden_request_py3.py
--rw-rw-rw-   0        0        0     1021 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_child.py
--rw-rw-rw-   0        0        0     1033 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_child_py3.py
--rw-rw-rw-   0        0        0     1030 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_response.py
--rw-rw-rw-   0        0        0     1042 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_response_py3.py
--rw-rw-rw-   0        0        0      895 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/target.py
--rw-rw-rw-   0        0        0      909 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_py3.py
--rw-rw-rw-   0        0        0     1457 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_settings.py
--rw-rw-rw-   0        0        0     1458 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_settings_py3.py
--rw-rw-rw-   0        0        0      884 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_edit.py
--rw-rw-rw-   0        0        0      891 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_edit_py3.py
--rw-rw-rw-   0        0        0     3923 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_response.py
--rw-rw-rw-   0        0        0     3933 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_response_py3.py
--rw-rw-rw-   0        0        0     1145 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_type.py
--rw-rw-rw-   0        0        0     1172 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_type_py3.py
--rw-rw-rw-   0        0        0     1071 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_child.py
--rw-rw-rw-   0        0        0     1095 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_child_py3.py
--rw-rw-rw-   0        0        0     2991 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_line.py
--rw-rw-rw-   0        0        0     3022 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_line_py3.py
--rw-rw-rw-   0        0        0     2008 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_response.py
--rw-rw-rw-   0        0        0     2012 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_response_py3.py
--rw-rw-rw-   0        0        0     1635 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_vendor_line_request.py
--rw-rw-rw-   0        0        0     1646 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_vendor_line_request_py3.py
--rw-rw-rw-   0        0        0     1665 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_version.py
--rw-rw-rw-   0        0        0     1674 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_version_py3.py
--rw-rw-rw-   0        0        0      954 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_format_response.py
--rw-rw-rw-   0        0        0      972 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_format_response_py3.py
--rw-rw-rw-   0        0        0      967 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_data_response.py
--rw-rw-rw-   0        0        0      966 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_data_response_py3.py
--rw-rw-rw-   0        0        0     1146 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_entity.py
--rw-rw-rw-   0        0        0     1155 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_entity_py3.py
--rw-rw-rw-   0        0        0     1308 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_value.py
--rw-rw-rw-   0        0        0     1315 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_value_py3.py
--rw-rw-rw-   0        0        0     1086 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_child.py
--rw-rw-rw-   0        0        0     1113 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_child_py3.py
--rw-rw-rw-   0        0        0     1670 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_response.py
--rw-rw-rw-   0        0        0     1719 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_response_py3.py
--rw-rw-rw-   0        0        0      743 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/toggle_visible.py
--rw-rw-rw-   0        0        0      754 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/toggle_visible_py3.py
--rw-rw-rw-   0        0        0     2201 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request.py
--rw-rw-rw-   0        0        0     2215 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request_py3.py
--rw-rw-rw-   0        0        0     2230 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response.py
--rw-rw-rw-   0        0        0     2259 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response_py3.py
--rw-rw-rw-   0        0        0     1844 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_cost_center.py
--rw-rw-rw-   0        0        0     1911 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_cost_center_py3.py
--rw-rw-rw-   0        0        0     1825 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_place.py
--rw-rw-rw-   0        0        0     1859 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_place_py3.py
--rw-rw-rw-   0        0        0     2165 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request.py
--rw-rw-rw-   0        0        0     2184 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request_py3.py
--rw-rw-rw-   0        0        0     2290 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response.py
--rw-rw-rw-   0        0        0     2324 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response_py3.py
--rw-rw-rw-   0        0        0     1947 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_data_response.py
--rw-rw-rw-   0        0        0     1947 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_data_response_py3.py
--rw-rw-rw-   0        0        0     1737 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_target.py
--rw-rw-rw-   0        0        0     1779 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_target_py3.py
--rw-rw-rw-   0        0        0     3144 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_create.py
--rw-rw-rw-   0        0        0     3144 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_create_py3.py
--rw-rw-rw-   0        0        0     2519 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_edit.py
--rw-rw-rw-   0        0        0     2525 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_edit_py3.py
--rw-rw-rw-   0        0        0     1927 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_field_child.py
--rw-rw-rw-   0        0        0     1934 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_field_child_py3.py
--rw-rw-rw-   0        0        0     2733 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_response.py
--rw-rw-rw-   0        0        0     2739 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_response_py3.py
--rw-rw-rw-   0        0        0     1368 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_create.py
--rw-rw-rw-   0        0        0     1371 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_create_py3.py
--rw-rw-rw-   0        0        0     1738 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_edit.py
--rw-rw-rw-   0        0        0     1752 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_edit_py3.py
--rw-rw-rw-   0        0        0     1302 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_entity_response.py
--rw-rw-rw-   0        0        0     1326 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_entity_response_py3.py
--rw-rw-rw-   0        0        0     1233 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_response.py
--rw-rw-rw-   0        0        0     1254 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_response_py3.py
--rw-rw-rw-   0        0        0     1415 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_update.py
--rw-rw-rw-   0        0        0     1429 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_update_py3.py
--rw-rw-rw-   0        0        0     2406 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_update.py
--rw-rw-rw-   0        0        0     2409 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_update_py3.py
--rw-rw-rw-   0        0        0      948 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_value.py
--rw-rw-rw-   0        0        0      954 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_value_py3.py
--rw-rw-rw-   0        0        0     1468 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit.py
--rw-rw-rw-   0        0        0     1035 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_child.py
--rw-rw-rw-   0        0        0     1047 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_child_py3.py
--rw-rw-rw-   0        0        0     1476 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_py3.py
--rw-rw-rw-   0        0        0     1187 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_response.py
--rw-rw-rw-   0        0        0     1195 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_response_py3.py
--rw-rw-rw-   0        0        0     2411 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings.py
--rw-rw-rw-   0        0        0     1290 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_class_permission.py
--rw-rw-rw-   0        0        0     1292 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2455 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_py3.py
--rw-rw-rw-   0        0        0     1071 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_type.py
--rw-rw-rw-   0        0        0     1098 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_type_py3.py
--rw-rw-rw-   0        0        0     1994 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills.py
--rw-rw-rw-   0        0        0      873 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_class_permission.py
--rw-rw-rw-   0        0        0      880 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_class_permission_py3.py
--rw-rw-rw-   0        0        0     2043 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_py3.py
--rw-rw-rw-   0        0        0     1729 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_batch_status_request.py
--rw-rw-rw-   0        0        0     1735 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_batch_status_request_py3.py
--rw-rw-rw-   0        0        0      956 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_result.py
--rw-rw-rw-   0        0        0      966 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_result_py3.py
--rw-rw-rw-   0        0        0     1883 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills.py
--rw-rw-rw-   0        0        0      762 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_class_permission.py
--rw-rw-rw-   0        0        0      772 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_class_permission_py3.py
--rw-rw-rw-   0        0        0     1935 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_py3.py
--rw-rw-rw-   0        0        0      753 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/updated_only_result.py
--rw-rw-rw-   0        0        0      763 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/updated_only_result_py3.py
--rw-rw-rw-   0        0        0     3283 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/upsert_aggregate_meter_request.py
--rw-rw-rw-   0        0        0     3307 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/upsert_aggregate_meter_request_py3.py
--rw-rw-rw-   0        0        0     1042 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child.py
--rw-rw-rw-   0        0        0     1054 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_py3.py
--rw-rw-rw-   0        0        0     1226 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_with_email.py
--rw-rw-rw-   0        0        0     1235 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_with_email_py3.py
--rw-rw-rw-   0        0        0     6659 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_create_request.py
--rw-rw-rw-   0        0        0     6719 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_create_request_py3.py
--rw-rw-rw-   0        0        0     8428 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_edit_request.py
--rw-rw-rw-   0        0        0     8478 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_edit_request_py3.py
--rw-rw-rw-   0        0        0      959 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_child.py
--rw-rw-rw-   0        0        0      982 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_child_py3.py
--rw-rw-rw-   0        0        0     2202 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_request.py
--rw-rw-rw-   0        0        0     2213 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_request_py3.py
--rw-rw-rw-   0        0        0     1642 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_response.py
--rw-rw-rw-   0        0        0     1671 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_response_py3.py
--rw-rw-rw-   0        0        0     1212 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_with_members.py
--rw-rw-rw-   0        0        0     1229 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_with_members_py3.py
--rw-rw-rw-   0        0        0     4386 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_response.py
--rw-rw-rw-   0        0        0     4444 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_response_py3.py
--rw-rw-rw-   0        0        0      816 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_role_request.py
--rw-rw-rw-   0        0        0      831 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_role_request_py3.py
--rw-rw-rw-   0        0        0     2301 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles.py
--rw-rw-rw-   0        0        0      855 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_class_permission.py
--rw-rw-rw-   0        0        0      862 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_class_permission_py3.py
--rw-rw-rw-   0        0        0     2350 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_py3.py
--rw-rw-rw-   0        0        0     1991 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups.py
--rw-rw-rw-   0        0        0      870 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_class_permission.py
--rw-rw-rw-   0        0        0      877 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_class_permission_py3.py
--rw-rw-rw-   0        0        0     2040 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_py3.py
--rw-rw-rw-   0        0        0      831 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform.py
--rw-rw-rw-   0        0        0     3576 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_meter.py
--rw-rw-rw-   0        0        0     3648 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_meter_py3.py
--rw-rw-rw-   0        0        0      855 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_py3.py
--rw-rw-rw-   0        0        0     1017 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_comparison.py
--rw-rw-rw-   0        0        0     1029 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_comparison_py3.py
--rw-rw-rw-   0        0        0      856 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_with_unit.py
--rw-rw-rw-   0        0        0      857 2023-04-26 10:27:17.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_with_unit_py3.py
--rw-rw-rw-   0        0        0      922 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_audit_enable.py
--rw-rw-rw-   0        0        0      939 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_audit_enable_py3.py
--rw-rw-rw-   0        0        0     1083 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_child.py
--rw-rw-rw-   0        0        0     1101 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_child_py3.py
--rw-rw-rw-   0        0        0     2674 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_contract_response.py
--rw-rw-rw-   0        0        0     2699 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_contract_response_py3.py
--rw-rw-rw-   0        0        0     2372 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response.py
--rw-rw-rw-   0        0        0     1966 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     1985 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     1810 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results.py
--rw-rw-rw-   0        0        0     1857 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results_py3.py
--rw-rw-rw-   0        0        0     2374 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1355 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_results.py
--rw-rw-rw-   0        0        0     1384 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     2492 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_request.py
--rw-rw-rw-   0        0        0     2502 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_request_py3.py
--rw-rw-rw-   0        0        0     3119 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_response.py
--rw-rw-rw-   0        0        0     3126 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_response_py3.py
--rw-rw-rw-   0        0        0      976 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_type_child.py
--rw-rw-rw-   0        0        0     1001 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_type_child_py3.py
--rw-rw-rw-   0        0        0     1320 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_udf_response.py
--rw-rw-rw-   0        0        0     1329 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_udf_response_py3.py
--rw-rw-rw-   0        0        0     2102 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors.py
--rw-rw-rw-   0        0        0     1856 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module.py
--rw-rw-rw-   0        0        0      735 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_class_permission.py
--rw-rw-rw-   0        0        0      743 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_class_permission_py3.py
--rw-rw-rw-   0        0        0     1906 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_py3.py
--rw-rw-rw-   0        0        0      981 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_class_permission.py
--rw-rw-rw-   0        0        0      987 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_class_permission_py3.py
--rw-rw-rw-   0        0        0     2150 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_py3.py
--rw-rw-rw-   0        0        0     1034 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_child.py
--rw-rw-rw-   0        0        0     1039 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_child_py3.py
--rw-rw-rw-   0        0        0     1043 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_response.py
--rw-rw-rw-   0        0        0     1048 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_response_py3.py
--rw-rw-rw-   0        0        0      807 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point.py
--rw-rw-rw-   0        0        0     1092 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_child.py
--rw-rw-rw-   0        0        0     1131 2023-04-26 10:27:16.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_child_py3.py
--rw-rw-rw-   0        0        0      831 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_py3.py
--rw-rw-rw-   0        0        0      927 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_request.py
--rw-rw-rw-   0        0        0      951 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_request_py3.py
--rw-rw-rw-   0        0        0      756 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site.py
--rw-rw-rw-   0        0        0      774 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_py3.py
--rw-rw-rw-   0        0        0      876 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_request.py
--rw-rw-rw-   0        0        0      894 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_request_py3.py
--rw-rw-rw-   0        0        0     1404 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_result.py
--rw-rw-rw-   0        0        0     1419 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_result_py3.py
--rw-rw-rw-   0        0        0     1333 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_settings.py
--rw-rw-rw-   0        0        0     1349 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_settings_py3.py
--rw-rw-rw-   0        0        0     1982 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings.py
--rw-rw-rw-   0        0        0      861 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_class_permission.py
--rw-rw-rw-   0        0        0      868 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_class_permission_py3.py
--rw-rw-rw-   0        0        0     2031 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_py3.py
--rw-rw-rw-   0        0        0     1658 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_child.py
--rw-rw-rw-   0        0        0     1671 2023-04-26 10:27:19.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_child_py3.py
--rw-rw-rw-   0        0        0     1607 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_response.py
--rw-rw-rw-   0        0        0     1631 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_response_py3.py
--rw-rw-rw-   0        0        0     3584 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_summary.py
--rw-rw-rw-   0        0        0     3712 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_summary_py3.py
--rw-rw-rw-   0        0        0     2718 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_create_request.py
--rw-rw-rw-   0        0        0     2724 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_create_request_py3.py
--rw-rw-rw-   0        0        0     1292 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_custom_action.py
--rw-rw-rw-   0        0        0     1290 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_custom_action_py3.py
--rw-rw-rw-   0        0        0     3080 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_edit_request.py
--rw-rw-rw-   0        0        0     3080 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_edit_request_py3.py
--rw-rw-rw-   0        0        0     1105 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_event_type_child.py
--rw-rw-rw-   0        0        0     1144 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_event_type_child_py3.py
--rw-rw-rw-   0        0        0     1872 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_details_response.py
--rw-rw-rw-   0        0        0     1866 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_details_response_py3.py
--rw-rw-rw-   0        0        0     1475 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_response.py
--rw-rw-rw-   0        0        0     1485 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_response_py3.py
--rw-rw-rw-   0        0        0     3185 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_response.py
--rw-rw-rw-   0        0        0     3209 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_response_py3.py
--rw-rw-rw-   0        0        0     2900 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_create.py
--rw-rw-rw-   0        0        0     2873 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_create_py3.py
--rw-rw-rw-   0        0        0     2946 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_edit.py
--rw-rw-rw-   0        0        0     2948 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_edit_py3.py
--rw-rw-rw-   0        0        0     1453 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_response.py
--rw-rw-rw-   0        0        0     1456 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_response_py3.py
--rw-rw-rw-   0        0        0     3997 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response.py
--rw-rw-rw-   0        0        0     2809 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_commodity_data.py
--rw-rw-rw-   0        0        0     2895 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_commodity_data_py3.py
--rw-rw-rw-   0        0        0     4083 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_py3.py
--rw-rw-rw-   0        0        0     1995 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_results.py
--rw-rw-rw-   0        0        0     2033 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_results_py3.py
--rw-rw-rw-   0        0        0     1818 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_display_setting.py
--rw-rw-rw-   0        0        0     1880 2023-04-26 10:27:18.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_display_setting_py3.py
--rw-rw-rw-   0        0        0     2075 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_request.py
--rw-rw-rw-   0        0        0     2050 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_request_py3.py
--rw-rw-rw-   0        0        0     1874 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_response.py
--rw-rw-rw-   0        0        0     1859 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_response_py3.py
--rw-rw-rw-   0        0        0      917 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/year_range.py
--rw-rw-rw-   0        0        0      930 2023-04-26 10:27:20.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/models/year_range_py3.py
--rw-rw-rw-   0        0        0      340 2023-04-26 10:27:15.000000 EnergyCapSdk-8.2302.4520/energycap/sdk/version.py
--rw-rw-rw-   0        0        0       42 2023-04-26 10:27:47.577684 EnergyCapSdk-8.2302.4520/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-04-26 10:27:14.000000 EnergyCapSdk-8.2302.4520/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:07:49.789930 EnergyCapSdk-8.2302.4532/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:07:28.861522 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-05-08 15:07:27.000000 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0   101423 2023-05-08 15:07:28.000000 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:07:27.000000 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-08 15:07:27.000000 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 15:07:27.000000 EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      293 2023-05-08 15:07:49.788765 EnergyCapSdk-8.2302.4532/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 15:07:28.869524 EnergyCapSdk-8.2302.4532/energycap/
+-rw-rw-rw-   0        0        0       56 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:07:29.029254 EnergyCapSdk-8.2302.4532/energycap/sdk/
+-rw-rw-rw-   0        0        0      437 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/__init__.py
+-rw-rw-rw-   0        0        0  1640151 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/energy_cap_api.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:07:49.785432 EnergyCapSdk-8.2302.4532/energycap/sdk/models/
+-rw-rw-rw-   0        0        0   165177 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request.py
+-rw-rw-rw-   0        0        0     2181 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2321 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response.py
+-rw-rw-rw-   0        0        0     2356 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response_py3.py
+-rw-rw-rw-   0        0        0     2174 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response.py
+-rw-rw-rw-   0        0        0     2369 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response_py3.py
+-rw-rw-rw-   0        0        0     2157 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request.py
+-rw-rw-rw-   0        0        0     2177 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2317 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response.py
+-rw-rw-rw-   0        0        0     2352 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1964 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_request.py
+-rw-rw-rw-   0        0        0     1960 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_request_py3.py
+-rw-rw-rw-   0        0        0     1426 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_response.py
+-rw-rw-rw-   0        0        0     1442 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_response_py3.py
+-rw-rw-rw-   0        0        0     1245 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_audit_enable.py
+-rw-rw-rw-   0        0        0     1260 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_audit_enable_py3.py
+-rw-rw-rw-   0        0        0     2068 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child.py
+-rw-rw-rw-   0        0        0     2123 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_py3.py
+-rw-rw-rw-   0        0        0     2317 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_with_type.py
+-rw-rw-rw-   0        0        0     2371 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_with_type_py3.py
+-rw-rw-rw-   0        0        0     1038 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_child.py
+-rw-rw-rw-   0        0        0     1057 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_child_py3.py
+-rw-rw-rw-   0        0        0     1913 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_request.py
+-rw-rw-rw-   0        0        0     1938 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_request_py3.py
+-rw-rw-rw-   0        0        0     1634 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_response.py
+-rw-rw-rw-   0        0        0     1662 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_response_py3.py
+-rw-rw-rw-   0        0        0     1158 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_connection_status_response.py
+-rw-rw-rw-   0        0        0     1191 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_connection_status_response_py3.py
+-rw-rw-rw-   0        0        0     8063 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_create.py
+-rw-rw-rw-   0        0        0     8083 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_create_py3.py
+-rw-rw-rw-   0        0        0     2409 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response.py
+-rw-rw-rw-   0        0        0     1987 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2006 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     2661 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     2735 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2414 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     2206 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_results.py
+-rw-rw-rw-   0        0        0     2262 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2400 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response.py
+-rw-rw-rw-   0        0        0     1971 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     1990 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1813 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1860 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2405 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1358 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1387 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     8385 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_edit.py
+-rw-rw-rw-   0        0        0     8414 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_edit_py3.py
+-rw-rw-rw-   0        0        0     3752 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child.py
+-rw-rw-rw-   0        0        0     3798 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_py3.py
+-rw-rw-rw-   0        0        0     4014 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_with_serial_number.py
+-rw-rw-rw-   0        0        0     4065 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_with_serial_number_py3.py
+-rw-rw-rw-   0        0        0     2008 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_edit.py
+-rw-rw-rw-   0        0        0     2026 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_edit_py3.py
+-rw-rw-rw-   0        0        0     2025 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_rate_response.py
+-rw-rw-rw-   0        0        0     2020 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_rate_response_py3.py
+-rw-rw-rw-   0        0        0     4081 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_request.py
+-rw-rw-rw-   0        0        0     4092 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_request_py3.py
+-rw-rw-rw-   0        0        0     3186 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_response.py
+-rw-rw-rw-   0        0        0     3179 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_response_py3.py
+-rw-rw-rw-   0        0        0     1186 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_or_meter_usage.py
+-rw-rw-rw-   0        0        0     1205 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_or_meter_usage_py3.py
+-rw-rw-rw-   0        0        0     1460 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_request.py
+-rw-rw-rw-   0        0        0     1467 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_request_py3.py
+-rw-rw-rw-   0        0        0     1148 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_response.py
+-rw-rw-rw-   0        0        0     1169 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_response_py3.py
+-rw-rw-rw-   0        0        0     1045 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_child.py
+-rw-rw-rw-   0        0        0     1039 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_child_py3.py
+-rw-rw-rw-   0        0        0     1378 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_request.py
+-rw-rw-rw-   0        0        0     1375 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_request_py3.py
+-rw-rw-rw-   0        0        0     1990 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_response.py
+-rw-rw-rw-   0        0        0     1970 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_response_py3.py
+-rw-rw-rw-   0        0        0     8130 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_response.py
+-rw-rw-rw-   0        0        0     8217 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_response_py3.py
+-rw-rw-rw-   0        0        0     2061 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_template_response.py
+-rw-rw-rw-   0        0        0     2079 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_template_response_py3.py
+-rw-rw-rw-   0        0        0     1221 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_type_child.py
+-rw-rw-rw-   0        0        0     1257 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_type_child_py3.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_udf_response.py
+-rw-rw-rw-   0        0        0     1356 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_udf_response_py3.py
+-rw-rw-rw-   0        0        0     1991 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings.py
+-rw-rw-rw-   0        0        0      870 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_class_permission.py
+-rw-rw-rw-   0        0        0      877 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2040 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_py3.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_request.py
+-rw-rw-rw-   0        0        0     2395 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_request_py3.py
+-rw-rw-rw-   0        0        0     1858 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_response.py
+-rw-rw-rw-   0        0        0     1919 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_response_py3.py
+-rw-rw-rw-   0        0        0     2237 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts.py
+-rw-rw-rw-   0        0        0     1116 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_class_permission.py
+-rw-rw-rw-   0        0        0     1119 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1835 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module.py
+-rw-rw-rw-   0        0        0     1865 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data.py
+-rw-rw-rw-   0        0        0      744 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_class_permission.py
+-rw-rw-rw-   0        0        0      752 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1915 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_py3.py
+-rw-rw-rw-   0        0        0      714 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_class_permission.py
+-rw-rw-rw-   0        0        0      722 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1885 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_py3.py
+-rw-rw-rw-   0        0        0     2282 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_py3.py
+-rw-rw-rw-   0        0        0     6206 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_processor_request.py
+-rw-rw-rw-   0        0        0     6321 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_processor_request_py3.py
+-rw-rw-rw-   0        0        0     2108 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings.py
+-rw-rw-rw-   0        0        0      987 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_class_permission.py
+-rw-rw-rw-   0        0        0      990 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2153 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_py3.py
+-rw-rw-rw-   0        0        0     2217 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_response.py
+-rw-rw-rw-   0        0        0     2269 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_response_py3.py
+-rw-rw-rw-   0        0        0     2070 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/actionable_bill_counts.py
+-rw-rw-rw-   0        0        0     2142 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/actionable_bill_counts_py3.py
+-rw-rw-rw-   0        0        0      779 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/activity.py
+-rw-rw-rw-   0        0        0      782 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/activity_py3.py
+-rw-rw-rw-   0        0        0     3685 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_child.py
+-rw-rw-rw-   0        0        0     3694 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_child_py3.py
+-rw-rw-rw-   0        0        0     2541 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_lookup.py
+-rw-rw-rw-   0        0        0     2574 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_lookup_py3.py
+-rw-rw-rw-   0        0        0     1356 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjusted_cost_type_response.py
+-rw-rw-rw-   0        0        0     1410 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjusted_cost_type_response_py3.py
+-rw-rw-rw-   0        0        0     1052 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjustment_base_method_child.py
+-rw-rw-rw-   0        0        0     1080 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjustment_base_method_child_py3.py
+-rw-rw-rw-   0        0        0     1884 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_request.py
+-rw-rw-rw-   0        0        0     1888 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_request_py3.py
+-rw-rw-rw-   0        0        0     1102 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_response.py
+-rw-rw-rw-   0        0        0     1108 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_response_py3.py
+-rw-rw-rw-   0        0        0     1352 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison.py
+-rw-rw-rw-   0        0        0     1353 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison_py3.py
+-rw-rw-rw-   0        0        0     1211 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_item_rank_response.py
+-rw-rw-rw-   0        0        0     1218 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_item_rank_response_py3.py
+-rw-rw-rw-   0        0        0     1098 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_monthly_cap_trend_response.py
+-rw-rw-rw-   0        0        0     1114 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_monthly_cap_trend_response_py3.py
+-rw-rw-rw-   0        0        0     1204 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_ghg_building_rank.py
+-rw-rw-rw-   0        0        0     1199 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_ghg_building_rank_py3.py
+-rw-rw-rw-   0        0        0     1267 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_item_rank_with_unit_response.py
+-rw-rw-rw-   0        0        0     1262 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_item_rank_with_unit_response_py3.py
+-rw-rw-rw-   0        0        0     1850 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports.py
+-rw-rw-rw-   0        0        0      729 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_class_permission.py
+-rw-rw-rw-   0        0        0      737 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1900 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_py3.py
+-rw-rw-rw-   0        0        0     1323 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_request.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_request_py3.py
+-rw-rw-rw-   0        0        0     1831 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_response.py
+-rw-rw-rw-   0        0        0     1854 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_response_py3.py
+-rw-rw-rw-   0        0        0     1380 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_edit_request.py
+-rw-rw-rw-   0        0        0     1401 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_edit_request_py3.py
+-rw-rw-rw-   0        0        0     1590 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_response.py
+-rw-rw-rw-   0        0        0     1614 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_response_py3.py
+-rw-rw-rw-   0        0        0      834 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_user.py
+-rw-rw-rw-   0        0        0      847 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_user_py3.py
+-rw-rw-rw-   0        0        0     1994 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_class_permission.py
+-rw-rw-rw-   0        0        0      880 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2043 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_py3.py
+-rw-rw-rw-   0        0        0     1105 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_child.py
+-rw-rw-rw-   0        0        0     1142 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_child_py3.py
+-rw-rw-rw-   0        0        0     1057 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_request_child.py
+-rw-rw-rw-   0        0        0     1075 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_request_child_py3.py
+-rw-rw-rw-   0        0        0     1261 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_settings.py
+-rw-rw-rw-   0        0        0     1313 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0     1841 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills.py
+-rw-rw-rw-   0        0        0      720 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_class_permission.py
+-rw-rw-rw-   0        0        0      730 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1893 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_py3.py
+-rw-rw-rw-   0        0        0      980 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/assign_versions_to_step.py
+-rw-rw-rw-   0        0        0     1004 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/assign_versions_to_step_py3.py
+-rw-rw-rw-   0        0        0     2222 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_request.py
+-rw-rw-rw-   0        0        0     2269 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_request_py3.py
+-rw-rw-rw-   0        0        0     2293 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_response.py
+-rw-rw-rw-   0        0        0     2340 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_response_py3.py
+-rw-rw-rw-   0        0        0     1574 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_request.py
+-rw-rw-rw-   0        0        0     1591 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_request_py3.py
+-rw-rw-rw-   0        0        0     1860 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_response.py
+-rw-rw-rw-   0        0        0     1892 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_response_py3.py
+-rw-rw-rw-   0        0        0    13015 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_request.py
+-rw-rw-rw-   0        0        0    13542 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_request_py3.py
+-rw-rw-rw-   0        0        0    11371 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_response.py
+-rw-rw-rw-   0        0        0    12003 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_response_py3.py
+-rw-rw-rw-   0        0        0     1829 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine.py
+-rw-rw-rw-   0        0        0      708 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_class_permission.py
+-rw-rw-rw-   0        0        0      715 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1878 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_py3.py
+-rw-rw-rw-   0        0        0     1588 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_log.py
+-rw-rw-rw-   0        0        0     1618 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_log_py3.py
+-rw-rw-rw-   0        0        0     4474 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request.py
+-rw-rw-rw-   0        0        0     1032 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_baseline_bill.py
+-rw-rw-rw-   0        0        0     1046 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_baseline_bill_py3.py
+-rw-rw-rw-   0        0        0     4575 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_py3.py
+-rw-rw-rw-   0        0        0    11293 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response.py
+-rw-rw-rw-   0        0        0     3493 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_baseline_bill.py
+-rw-rw-rw-   0        0        0     3559 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_baseline_bill_py3.py
+-rw-rw-rw-   0        0        0    11696 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_py3.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_child.py
+-rw-rw-rw-   0        0        0      886 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_child_py3.py
+-rw-rw-rw-   0        0        0     4045 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_create.py
+-rw-rw-rw-   0        0        0     4091 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_create_py3.py
+-rw-rw-rw-   0        0        0     1376 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_edit.py
+-rw-rw-rw-   0        0        0     1380 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_edit_py3.py
+-rw-rw-rw-   0        0        0     5049 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_response.py
+-rw-rw-rw-   0        0        0     5135 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_response_py3.py
+-rw-rw-rw-   0        0        0     2159 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_settings.py
+-rw-rw-rw-   0        0        0     2186 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_settings_py3.py
+-rw-rw-rw-   0        0        0     2802 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_child.py
+-rw-rw-rw-   0        0        0     2785 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_child_py3.py
+-rw-rw-rw-   0        0        0     2527 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_settings.py
+-rw-rw-rw-   0        0        0     2556 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0     1088 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_category_response.py
+-rw-rw-rw-   0        0        0     1127 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_category_response_py3.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_edit.py
+-rw-rw-rw-   0        0        0     1453 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_edit_py3.py
+-rw-rw-rw-   0        0        0     1182 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_edit.py
+-rw-rw-rw-   0        0        0     1184 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_edit_py3.py
+-rw-rw-rw-   0        0        0     1296 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_response.py
+-rw-rw-rw-   0        0        0     1298 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_response_py3.py
+-rw-rw-rw-   0        0        0     1649 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value.py
+-rw-rw-rw-   0        0        0     1665 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_py3.py
+-rw-rw-rw-   0        0        0     1674 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_request.py
+-rw-rw-rw-   0        0        0     1675 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_request_py3.py
+-rw-rw-rw-   0        0        0     1796 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_values_response.py
+-rw-rw-rw-   0        0        0     1832 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_values_response_py3.py
+-rw-rw-rw-   0        0        0     1523 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_with_used_count_response.py
+-rw-rw-rw-   0        0        0     1558 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_with_used_count_response_py3.py
+-rw-rw-rw-   0        0        0     2076 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_create.py
+-rw-rw-rw-   0        0        0     2098 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_create_py3.py
+-rw-rw-rw-   0        0        0     2536 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_edit.py
+-rw-rw-rw-   0        0        0     2562 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_edit_py3.py
+-rw-rw-rw-   0        0        0     3745 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_child.py
+-rw-rw-rw-   0        0        0     3863 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_child_py3.py
+-rw-rw-rw-   0        0        0     7951 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_response.py
+-rw-rw-rw-   0        0        0     8167 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_response_py3.py
+-rw-rw-rw-   0        0        0     2574 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_statistics_response.py
+-rw-rw-rw-   0        0        0     2562 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_statistics_response_py3.py
+-rw-rw-rw-   0        0        0     1337 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_accrual_exclusion_request.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_accrual_exclusion_request_py3.py
+-rw-rw-rw-   0        0        0     1006 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_approve.py
+-rw-rw-rw-   0        0        0     1007 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_approve_py3.py
+-rw-rw-rw-   0        0        0     1319 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_custom.py
+-rw-rw-rw-   0        0        0     1322 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_custom_py3.py
+-rw-rw-rw-   0        0        0      731 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_delete.py
+-rw-rw-rw-   0        0        0      732 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_delete_py3.py
+-rw-rw-rw-   0        0        0     1043 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_export_hold.py
+-rw-rw-rw-   0        0        0     1048 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_export_hold_py3.py
+-rw-rw-rw-   0        0        0     1305 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_header_update.py
+-rw-rw-rw-   0        0        0     1299 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_header_update_py3.py
+-rw-rw-rw-   0        0        0      943 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_historical_export.py
+-rw-rw-rw-   0        0        0      939 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_historical_export_py3.py
+-rw-rw-rw-   0        0        0     2018 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move.py
+-rw-rw-rw-   0        0        0     1750 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_list.py
+-rw-rw-rw-   0        0        0     1787 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_list_py3.py
+-rw-rw-rw-   0        0        0     2045 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_py3.py
+-rw-rw-rw-   0        0        0     1149 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_split.py
+-rw-rw-rw-   0        0        0     1147 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_split_py3.py
+-rw-rw-rw-   0        0        0      979 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_void.py
+-rw-rw-rw-   0        0        0      977 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_void_py3.py
+-rw-rw-rw-   0        0        0     3784 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_calendarized_history.py
+-rw-rw-rw-   0        0        0     3848 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_calendarized_history_py3.py
+-rw-rw-rw-   0        0        0     2248 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request.py
+-rw-rw-rw-   0        0        0     2274 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2373 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response.py
+-rw-rw-rw-   0        0        0     2414 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response_py3.py
+-rw-rw-rw-   0        0        0     2126 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_request.py
+-rw-rw-rw-   0        0        0     2145 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2251 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_response.py
+-rw-rw-rw-   0        0        0     2285 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_response_py3.py
+-rw-rw-rw-   0        0        0     5406 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_create.py
+-rw-rw-rw-   0        0        0     5404 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_create_py3.py
+-rw-rw-rw-   0        0        0      863 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_delete_action_result.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_delete_action_result_py3.py
+-rw-rw-rw-   0        0        0     6222 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_edit.py
+-rw-rw-rw-   0        0        0     6230 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_edit_py3.py
+-rw-rw-rw-   0        0        0     1601 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line.py
+-rw-rw-rw-   0        0        0     1058 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_child.py
+-rw-rw-rw-   0        0        0     1055 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_child_py3.py
+-rw-rw-rw-   0        0        0     1601 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_py3.py
+-rw-rw-rw-   0        0        0     1233 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_with_noun_child.py
+-rw-rw-rw-   0        0        0     1226 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_with_noun_child_py3.py
+-rw-rw-rw-   0        0        0     1894 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_meter_child.py
+-rw-rw-rw-   0        0        0     1923 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_meter_child_py3.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_observation_type_child.py
+-rw-rw-rw-   0        0        0     1392 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_observation_type_child_py3.py
+-rw-rw-rw-   0        0        0     8971 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_response.py
+-rw-rw-rw-   0        0        0     9045 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_response_py3.py
+-rw-rw-rw-   0        0        0     1869 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export.py
+-rw-rw-rw-   0        0        0     1555 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_options.py
+-rw-rw-rw-   0        0        0     1571 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_options_py3.py
+-rw-rw-rw-   0        0        0     1880 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_py3.py
+-rw-rw-rw-   0        0        0      918 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_child.py
+-rw-rw-rw-   0        0        0      927 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_child_py3.py
+-rw-rw-rw-   0        0        0     3433 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update.py
+-rw-rw-rw-   0        0        0     1379 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_account_period_child.py
+-rw-rw-rw-   0        0        0     1390 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_account_period_child_py3.py
+-rw-rw-rw-   0        0        0     1310 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_begin_date_child.py
+-rw-rw-rw-   0        0        0     1312 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_begin_date_child_py3.py
+-rw-rw-rw-   0        0        0     1252 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_billing_period_child.py
+-rw-rw-rw-   0        0        0     1263 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_billing_period_child_py3.py
+-rw-rw-rw-   0        0        0     1360 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_control_code_child.py
+-rw-rw-rw-   0        0        0     1369 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_control_code_child_py3.py
+-rw-rw-rw-   0        0        0     1275 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_due_date_child.py
+-rw-rw-rw-   0        0        0     1275 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_due_date_child_py3.py
+-rw-rw-rw-   0        0        0     1292 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_end_date_child.py
+-rw-rw-rw-   0        0        0     1292 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_end_date_child_py3.py
+-rw-rw-rw-   0        0        0     1212 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_estimated_child.py
+-rw-rw-rw-   0        0        0     1219 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_estimated_child_py3.py
+-rw-rw-rw-   0        0        0     1378 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_invoice_number_child.py
+-rw-rw-rw-   0        0        0     1389 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_invoice_number_child_py3.py
+-rw-rw-rw-   0        0        0     3385 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_py3.py
+-rw-rw-rw-   0        0        0     1329 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_statement_date_child.py
+-rw-rw-rw-   0        0        0     1335 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_statement_date_child_py3.py
+-rw-rw-rw-   0        0        0      881 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_workflow_child.py
+-rw-rw-rw-   0        0        0      895 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_workflow_child_py3.py
+-rw-rw-rw-   0        0        0     3431 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_history_response.py
+-rw-rw-rw-   0        0        0     3451 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_history_response_py3.py
+-rw-rw-rw-   0        0        0      704 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_id_response.py
+-rw-rw-rw-   0        0        0      714 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_id_response_py3.py
+-rw-rw-rw-   0        0        0     9204 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_column_mapping.py
+-rw-rw-rw-   0        0        0     9494 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_column_mapping_py3.py
+-rw-rw-rw-   0        0        0     2051 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_observation.py
+-rw-rw-rw-   0        0        0     2059 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_observation_py3.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_request.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_request_py3.py
+-rw-rw-rw-   0        0        0     1634 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_response.py
+-rw-rw-rw-   0        0        0     1647 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_response_py3.py
+-rw-rw-rw-   0        0        0     2737 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_request.py
+-rw-rw-rw-   0        0        0     2751 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_request_py3.py
+-rw-rw-rw-   0        0        0      920 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_workflow_settings.py
+-rw-rw-rw-   0        0        0      937 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0     1868 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator.py
+-rw-rw-rw-   0        0        0      747 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_class_permission.py
+-rw-rw-rw-   0        0        0      757 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1920 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_py3.py
+-rw-rw-rw-   0        0        0     2173 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_create.py
+-rw-rw-rw-   0        0        0     2190 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_create_py3.py
+-rw-rw-rw-   0        0        0     2701 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_edit.py
+-rw-rw-rw-   0        0        0     2722 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_edit_py3.py
+-rw-rw-rw-   0        0        0     1339 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_create.py
+-rw-rw-rw-   0        0        0     1337 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_create_py3.py
+-rw-rw-rw-   0        0        0     1329 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_edit.py
+-rw-rw-rw-   0        0        0     1327 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_edit_py3.py
+-rw-rw-rw-   0        0        0     1461 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_file_response.py
+-rw-rw-rw-   0        0        0     1476 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_file_response_py3.py
+-rw-rw-rw-   0        0        0     3854 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_item.py
+-rw-rw-rw-   0        0        0     3854 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_item_py3.py
+-rw-rw-rw-   0        0        0     1569 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_response.py
+-rw-rw-rw-   0        0        0     1591 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_response_py3.py
+-rw-rw-rw-   0        0        0    12793 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_response.py
+-rw-rw-rw-   0        0        0    12915 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_response_py3.py
+-rw-rw-rw-   0        0        0     1391 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal.py
+-rw-rw-rw-   0        0        0     1420 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_py3.py
+-rw-rw-rw-   0        0        0     1224 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_request.py
+-rw-rw-rw-   0        0        0     1226 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_request_py3.py
+-rw-rw-rw-   0        0        0     2225 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request.py
+-rw-rw-rw-   0        0        0     2257 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2350 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response.py
+-rw-rw-rw-   0        0        0     2397 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response_py3.py
+-rw-rw-rw-   0        0        0     2497 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_request.py
+-rw-rw-rw-   0        0        0     2531 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_request_py3.py
+-rw-rw-rw-   0        0        0     2020 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_response.py
+-rw-rw-rw-   0        0        0     2048 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_response_py3.py
+-rw-rw-rw-   0        0        0     1555 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_parent_details_response.py
+-rw-rw-rw-   0        0        0     1584 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_parent_details_response_py3.py
+-rw-rw-rw-   0        0        0     1388 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_place_size_child.py
+-rw-rw-rw-   0        0        0     1386 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_place_size_child_py3.py
+-rw-rw-rw-   0        0        0     1294 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport.py
+-rw-rw-rw-   0        0        0      990 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_options.py
+-rw-rw-rw-   0        0        0      999 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_options_py3.py
+-rw-rw-rw-   0        0        0     1293 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_py3.py
+-rw-rw-rw-   0        0        0     1341 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_usage.py
+-rw-rw-rw-   0        0        0     1361 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_usage_py3.py
+-rw-rw-rw-   0        0        0     2125 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_account_child.py
+-rw-rw-rw-   0        0        0     2139 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_account_child_py3.py
+-rw-rw-rw-   0        0        0     1955 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_address_child.py
+-rw-rw-rw-   0        0        0     1959 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_address_child_py3.py
+-rw-rw-rw-   0        0        0     2282 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_meter_child.py
+-rw-rw-rw-   0        0        0     2279 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_meter_child_py3.py
+-rw-rw-rw-   0        0        0    15009 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_response.py
+-rw-rw-rw-   0        0        0    15189 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_response_py3.py
+-rw-rw-rw-   0        0        0     1311 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_vendor_child.py
+-rw-rw-rw-   0        0        0     1323 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_vendor_child_py3.py
+-rw-rw-rw-   0        0        0     1997 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings.py
+-rw-rw-rw-   0        0        0      876 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_class_permission.py
+-rw-rw-rw-   0        0        0      883 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2046 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0      887 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_child.py
+-rw-rw-rw-   0        0        0      887 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_child_py3.py
+-rw-rw-rw-   0        0        0     1149 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_delta_child.py
+-rw-rw-rw-   0        0        0     1148 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_delta_child_py3.py
+-rw-rw-rw-   0        0        0     2300 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_child.py
+-rw-rw-rw-   0        0        0     2354 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_child_py3.py
+-rw-rw-rw-   0        0        0     1355 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_delta_child.py
+-rw-rw-rw-   0        0        0     1353 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_delta_child_py3.py
+-rw-rw-rw-   0        0        0      884 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_child.py
+-rw-rw-rw-   0        0        0      883 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_child_py3.py
+-rw-rw-rw-   0        0        0     1097 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_delta_child.py
+-rw-rw-rw-   0        0        0     1095 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_delta_child_py3.py
+-rw-rw-rw-   0        0        0     2402 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches.py
+-rw-rw-rw-   0        0        0     1281 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_class_permission.py
+-rw-rw-rw-   0        0        0     1283 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2446 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_py3.py
+-rw-rw-rw-   0        0        0     1826 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module.py
+-rw-rw-rw-   0        0        0      705 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_class_permission.py
+-rw-rw-rw-   0        0        0      713 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1876 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_py3.py
+-rw-rw-rw-   0        0        0     1804 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_overdue_from_vendor_response.py
+-rw-rw-rw-   0        0        0     1799 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_overdue_from_vendor_response_py3.py
+-rw-rw-rw-   0        0        0     3173 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_child.py
+-rw-rw-rw-   0        0        0     3209 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_child_py3.py
+-rw-rw-rw-   0        0        0     3182 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_response.py
+-rw-rw-rw-   0        0        0     3169 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_response_py3.py
+-rw-rw-rw-   0        0        0     2285 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions.py
+-rw-rw-rw-   0        0        0     1164 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_class_permission.py
+-rw-rw-rw-   0        0        0     1167 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2330 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_py3.py
+-rw-rw-rw-   0        0        0     2147 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups.py
+-rw-rw-rw-   0        0        0     1026 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_class_permission.py
+-rw-rw-rw-   0        0        0     1032 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2195 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_py3.py
+-rw-rw-rw-   0        0        0     1865 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module.py
+-rw-rw-rw-   0        0        0     1895 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data.py
+-rw-rw-rw-   0        0        0      774 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission.py
+-rw-rw-rw-   0        0        0      782 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_py3.py
+-rw-rw-rw-   0        0        0     1913 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data.py
+-rw-rw-rw-   0        0        0      792 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission.py
+-rw-rw-rw-   0        0        0      800 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1963 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_py3.py
+-rw-rw-rw-   0        0        0      744 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_class_permission.py
+-rw-rw-rw-   0        0        0      752 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1916 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data.py
+-rw-rw-rw-   0        0        0      795 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission.py
+-rw-rw-rw-   0        0        0      803 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1966 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_py3.py
+-rw-rw-rw-   0        0        0     1907 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data.py
+-rw-rw-rw-   0        0        0      786 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission.py
+-rw-rw-rw-   0        0        0      794 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1957 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_py3.py
+-rw-rw-rw-   0        0        0     1915 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_py3.py
+-rw-rw-rw-   0        0        0     1886 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings.py
+-rw-rw-rw-   0        0        0      765 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_class_permission.py
+-rw-rw-rw-   0        0        0      773 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1936 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_py3.py
+-rw-rw-rw-   0        0        0     1907 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability.py
+-rw-rw-rw-   0        0        0      786 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission.py
+-rw-rw-rw-   0        0        0      794 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1957 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_py3.py
+-rw-rw-rw-   0        0        0     2288 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations.py
+-rw-rw-rw-   0        0        0     1167 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_class_permission.py
+-rw-rw-rw-   0        0        0     1170 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2333 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_py3.py
+-rw-rw-rw-   0        0        0     1303 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_baseline_processor_request.py
+-rw-rw-rw-   0        0        0     1327 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_baseline_processor_request_py3.py
+-rw-rw-rw-   0        0        0     4384 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_meter_cost_avoidance_settings.py
+-rw-rw-rw-   0        0        0     4497 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_meter_cost_avoidance_settings_py3.py
+-rw-rw-rw-   0        0        0     3123 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculate_savings_request.py
+-rw-rw-rw-   0        0        0     3197 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculate_savings_request_py3.py
+-rw-rw-rw-   0        0        0     2972 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_request.py
+-rw-rw-rw-   0        0        0     3052 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_request_py3.py
+-rw-rw-rw-   0        0        0     2451 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_response.py
+-rw-rw-rw-   0        0        0     2503 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_response_py3.py
+-rw-rw-rw-   0        0        0     1488 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_request.py
+-rw-rw-rw-   0        0        0     1524 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_request_py3.py
+-rw-rw-rw-   0        0        0     1480 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_response.py
+-rw-rw-rw-   0        0        0     1517 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_response_py3.py
+-rw-rw-rw-   0        0        0     2326 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_details_response.py
+-rw-rw-rw-   0        0        0     2313 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_details_response_py3.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_request.py
+-rw-rw-rw-   0        0        0     2496 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_request_py3.py
+-rw-rw-rw-   0        0        0     2377 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_response.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_response_py3.py
+-rw-rw-rw-   0        0        0     1015 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_request.py
+-rw-rw-rw-   0        0        0     1011 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_request_py3.py
+-rw-rw-rw-   0        0        0     1118 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_response.py
+-rw-rw-rw-   0        0        0     1114 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_response_py3.py
+-rw-rw-rw-   0        0        0      819 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_request.py
+-rw-rw-rw-   0        0        0      820 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_request_py3.py
+-rw-rw-rw-   0        0        0      888 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_response.py
+-rw-rw-rw-   0        0        0      902 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_response_py3.py
+-rw-rw-rw-   0        0        0     1116 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_sum_request.py
+-rw-rw-rw-   0        0        0     1122 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_sum_request_py3.py
+-rw-rw-rw-   0        0        0     1351 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child.py
+-rw-rw-rw-   0        0        0     1368 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_py3.py
+-rw-rw-rw-   0        0        0     1770 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_with_observation_type.py
+-rw-rw-rw-   0        0        0     1769 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_with_observation_type_py3.py
+-rw-rw-rw-   0        0        0     2674 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_create.py
+-rw-rw-rw-   0        0        0     2713 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_create_py3.py
+-rw-rw-rw-   0        0        0     2828 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_edit.py
+-rw-rw-rw-   0        0        0     2872 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_edit_py3.py
+-rw-rw-rw-   0        0        0     1556 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_latest_reading.py
+-rw-rw-rw-   0        0        0     1571 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_latest_reading_py3.py
+-rw-rw-rw-   0        0        0     3383 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_response.py
+-rw-rw-rw-   0        0        0     3452 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_response_py3.py
+-rw-rw-rw-   0        0        0     2747 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_request.py
+-rw-rw-rw-   0        0        0     2751 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_request_py3.py
+-rw-rw-rw-   0        0        0     2309 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_response.py
+-rw-rw-rw-   0        0        0     2320 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_response_py3.py
+-rw-rw-rw-   0        0        0     3091 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_with_begin_date_request.py
+-rw-rw-rw-   0        0        0     3092 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_with_begin_date_request_py3.py
+-rw-rw-rw-   0        0        0     2867 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings.py
+-rw-rw-rw-   0        0        0     1240 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_aggregations.py
+-rw-rw-rw-   0        0        0     1254 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_aggregations_py3.py
+-rw-rw-rw-   0        0        0      982 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_splits.py
+-rw-rw-rw-   0        0        0      990 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_splits_py3.py
+-rw-rw-rw-   0        0        0     2880 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_py3.py
+-rw-rw-rw-   0        0        0     2563 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_without_filters.py
+-rw-rw-rw-   0        0        0     2582 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_without_filters_py3.py
+-rw-rw-rw-   0        0        0     1862 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals.py
+-rw-rw-rw-   0        0        0      741 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_class_permission.py
+-rw-rw-rw-   0        0        0      751 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1914 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_py3.py
+-rw-rw-rw-   0        0        0      936 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_request.py
+-rw-rw-rw-   0        0        0      941 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_request_py3.py
+-rw-rw-rw-   0        0        0     4421 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_response.py
+-rw-rw-rw-   0        0        0     4471 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_response_py3.py
+-rw-rw-rw-   0        0        0     5239 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_version_response.py
+-rw-rw-rw-   0        0        0     5292 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_version_response_py3.py
+-rw-rw-rw-   0        0        0     1122 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_base.py
+-rw-rw-rw-   0        0        0     1163 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_base_py3.py
+-rw-rw-rw-   0        0        0     1713 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_create.py
+-rw-rw-rw-   0        0        0     1747 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_create_py3.py
+-rw-rw-rw-   0        0        0     2045 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_child.py
+-rw-rw-rw-   0        0        0     2038 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_child_py3.py
+-rw-rw-rw-   0        0        0     1238 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_response.py
+-rw-rw-rw-   0        0        0     1254 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_response_py3.py
+-rw-rw-rw-   0        0        0     1518 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_split_child.py
+-rw-rw-rw-   0        0        0     1518 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_split_child_py3.py
+-rw-rw-rw-   0        0        0     1766 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_edit.py
+-rw-rw-rw-   0        0        0     1800 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_edit_py3.py
+-rw-rw-rw-   0        0        0     1497 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_response.py
+-rw-rw-rw-   0        0        0     1550 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_response_py3.py
+-rw-rw-rw-   0        0        0     1228 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_settings.py
+-rw-rw-rw-   0        0        0     1261 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0     2300 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step.py
+-rw-rw-rw-   0        0        0     2703 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_child.py
+-rw-rw-rw-   0        0        0     2831 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_child_py3.py
+-rw-rw-rw-   0        0        0     2282 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_create.py
+-rw-rw-rw-   0        0        0     2353 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_create_py3.py
+-rw-rw-rw-   0        0        0     2998 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_edit.py
+-rw-rw-rw-   0        0        0     3088 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_edit_py3.py
+-rw-rw-rw-   0        0        0     2422 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_py3.py
+-rw-rw-rw-   0        0        0     1964 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks.py
+-rw-rw-rw-   0        0        0      843 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_class_permission.py
+-rw-rw-rw-   0        0        0      849 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module.py
+-rw-rw-rw-   0        0        0      723 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_class_permission.py
+-rw-rw-rw-   0        0        0      731 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1894 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_py3.py
+-rw-rw-rw-   0        0        0     2012 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_py3.py
+-rw-rw-rw-   0        0        0      837 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/claim.py
+-rw-rw-rw-   0        0        0      847 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/claim_py3.py
+-rw-rw-rw-   0        0        0     1872 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_child.py
+-rw-rw-rw-   0        0        0     1371 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_child_py3.py
+-rw-rw-rw-   0        0        0     1838 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2000 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1819 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1866 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     1833 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1364 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1393 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1915 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_py3.py
+-rw-rw-rw-   0        0        0     1249 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_value_comparison.py
+-rw-rw-rw-   0        0        0     1257 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_value_comparison_py3.py
+-rw-rw-rw-   0        0        0     1202 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/contact_child.py
+-rw-rw-rw-   0        0        0     1206 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/contact_child_py3.py
+-rw-rw-rw-   0        0        0     1002 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_from_meter_response.py
+-rw-rw-rw-   0        0        0     1009 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_from_meter_response_py3.py
+-rw-rw-rw-   0        0        0     1732 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_meter_request.py
+-rw-rw-rw-   0        0        0     1737 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_meter_request_py3.py
+-rw-rw-rw-   0        0        0     3353 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_settings.py
+-rw-rw-rw-   0        0        0     3465 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_settings_py3.py
+-rw-rw-rw-   0        0        0     4158 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_task.py
+-rw-rw-rw-   0        0        0     4154 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_task_py3.py
+-rw-rw-rw-   0        0        0     2421 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_account_child.py
+-rw-rw-rw-   0        0        0     2482 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_account_child_py3.py
+-rw-rw-rw-   0        0        0     1197 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_child.py
+-rw-rw-rw-   0        0        0     1230 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_child_py3.py
+-rw-rw-rw-   0        0        0     2098 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_create.py
+-rw-rw-rw-   0        0        0     2123 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_create_py3.py
+-rw-rw-rw-   0        0        0     2508 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response.py
+-rw-rw-rw-   0        0        0     2002 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2021 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     2670 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     2744 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2525 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     2215 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_results.py
+-rw-rw-rw-   0        0        0     2271 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2499 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response.py
+-rw-rw-rw-   0        0        0     1986 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2005 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1822 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1869 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2516 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1367 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1396 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1905 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_response.py
+-rw-rw-rw-   0        0        0     1925 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_response_py3.py
+-rw-rw-rw-   0        0        0     2246 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers.py
+-rw-rw-rw-   0        0        0     1125 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_class_permission.py
+-rw-rw-rw-   0        0        0     1128 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2291 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_py3.py
+-rw-rw-rw-   0        0        0     1000 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_child.py
+-rw-rw-rw-   0        0        0     1021 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_child_py3.py
+-rw-rw-rw-   0        0        0     1327 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_unit.py
+-rw-rw-rw-   0        0        0     1378 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_unit_py3.py
+-rw-rw-rw-   0        0        0     1203 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/country.py
+-rw-rw-rw-   0        0        0     1220 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/country_py3.py
+-rw-rw-rw-   0        0        0     1404 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_template_from_bill.py
+-rw-rw-rw-   0        0        0     1411 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_template_from_bill_py3.py
+-rw-rw-rw-   0        0        0     1074 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_utility_platform_meter.py
+-rw-rw-rw-   0        0        0     1082 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_utility_platform_meter_py3.py
+-rw-rw-rw-   0        0        0     1131 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_child.py
+-rw-rw-rw-   0        0        0     1155 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_child_py3.py
+-rw-rw-rw-   0        0        0     1328 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_response.py
+-rw-rw-rw-   0        0        0     1346 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_response_py3.py
+-rw-rw-rw-   0        0        0     1871 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator.py
+-rw-rw-rw-   0        0        0      750 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_class_permission.py
+-rw-rw-rw-   0        0        0      760 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1923 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_py3.py
+-rw-rw-rw-   0        0        0     1859 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module.py
+-rw-rw-rw-   0        0        0      738 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_class_permission.py
+-rw-rw-rw-   0        0        0      746 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1909 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_py3.py
+-rw-rw-rw-   0        0        0     1646 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_copy.py
+-rw-rw-rw-   0        0        0     1665 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_copy_py3.py
+-rw-rw-rw-   0        0        0     1815 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_create.py
+-rw-rw-rw-   0        0        0     1825 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_create_py3.py
+-rw-rw-rw-   0        0        0     2036 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_edit.py
+-rw-rw-rw-   0        0        0     2041 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_edit_py3.py
+-rw-rw-rw-   0        0        0     2766 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_edit.py
+-rw-rw-rw-   0        0        0     3024 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_edit_py3.py
+-rw-rw-rw-   0        0        0     2809 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_py3.py
+-rw-rw-rw-   0        0        0     3497 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_response.py
+-rw-rw-rw-   0        0        0     3516 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_response_py3.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release.py
+-rw-rw-rw-   0        0        0     1130 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_meta_data.py
+-rw-rw-rw-   0        0        0     1158 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_meta_data_py3.py
+-rw-rw-rw-   0        0        0     1639 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_no_file_request.py
+-rw-rw-rw-   0        0        0     1652 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_no_file_request_py3.py
+-rw-rw-rw-   0        0        0     1874 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_py3.py
+-rw-rw-rw-   0        0        0     1994 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_request.py
+-rw-rw-rw-   0        0        0     2016 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_request_py3.py
+-rw-rw-rw-   0        0        0     1110 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_state.py
+-rw-rw-rw-   0        0        0     1123 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_state_py3.py
+-rw-rw-rw-   0        0        0     1399 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_status.py
+-rw-rw-rw-   0        0        0     1454 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_status_py3.py
+-rw-rw-rw-   0        0        0     1287 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_type_response.py
+-rw-rw-rw-   0        0        0     1314 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_type_response_py3.py
+-rw-rw-rw-   0        0        0      987 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/delete_reading_response.py
+-rw-rw-rw-   0        0        0      992 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/delete_reading_response_py3.py
+-rw-rw-rw-   0        0        0     1877 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_meter_child.py
+-rw-rw-rw-   0        0        0     1896 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_meter_child_py3.py
+-rw-rw-rw-   0        0        0     1863 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_response.py
+-rw-rw-rw-   0        0        0     1870 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_response_py3.py
+-rw-rw-rw-   0        0        0      750 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_base.py
+-rw-rw-rw-   0        0        0      764 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_base_py3.py
+-rw-rw-rw-   0        0        0     1148 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_to_bills_request.py
+-rw-rw-rw-   0        0        0     1157 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_to_bills_request_py3.py
+-rw-rw-rw-   0        0        0     3951 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_configuration.py
+-rw-rw-rw-   0        0        0     3976 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_configuration_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings.py
+-rw-rw-rw-   0        0        0      762 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_class_permission.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1935 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_py3.py
+-rw-rw-rw-   0        0        0     3340 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_manage.py
+-rw-rw-rw-   0        0        0     3360 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_manage_py3.py
+-rw-rw-rw-   0        0        0     2589 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_response.py
+-rw-rw-rw-   0        0        0     2602 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_response_py3.py
+-rw-rw-rw-   0        0        0     2183 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request.py
+-rw-rw-rw-   0        0        0     2196 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2213 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response.py
+-rw-rw-rw-   0        0        0     2241 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1132 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_list_request.py
+-rw-rw-rw-   0        0        0     1143 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_list_request_py3.py
+-rw-rw-rw-   0        0        0     2193 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split.py
+-rw-rw-rw-   0        0        0     2235 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_py3.py
+-rw-rw-rw-   0        0        0     1640 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_response.py
+-rw-rw-rw-   0        0        0     1689 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_response_py3.py
+-rw-rw-rw-   0        0        0     1247 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/email_properties.py
+-rw-rw-rw-   0        0        0     1245 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/email_properties_py3.py
+-rw-rw-rw-   0        0        0      950 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_cap_options_energy_cap_id_options.py
+-rw-rw-rw-   0        0        0      969 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_cap_options_energy_cap_id_options_py3.py
+-rw-rw-rw-   0        0        0     4814 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_create.py
+-rw-rw-rw-   0        0        0     4938 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_create_py3.py
+-rw-rw-rw-   0        0        0     5564 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_edit.py
+-rw-rw-rw-   0        0        0     5688 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_edit_py3.py
+-rw-rw-rw-   0        0        0     1098 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_place_child.py
+-rw-rw-rw-   0        0        0     1113 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_place_child_py3.py
+-rw-rw-rw-   0        0        0     4719 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_response.py
+-rw-rw-rw-   0        0        0     4795 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_response_py3.py
+-rw-rw-rw-   0        0        0     1369 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type.py
+-rw-rw-rw-   0        0        0     1686 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_create.py
+-rw-rw-rw-   0        0        0     1719 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_create_py3.py
+-rw-rw-rw-   0        0        0     1426 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_py3.py
+-rw-rw-rw-   0        0        0     1036 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_child.py
+-rw-rw-rw-   0        0        0     1061 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_child_py3.py
+-rw-rw-rw-   0        0        0     1375 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_unit.py
+-rw-rw-rw-   0        0        0     1432 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_unit_py3.py
+-rw-rw-rw-   0        0        0     1861 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping.py
+-rw-rw-rw-   0        0        0     1693 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child.py
+-rw-rw-rw-   0        0        0     1735 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child_py3.py
+-rw-rw-rw-   0        0        0     1912 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_py3.py
+-rw-rw-rw-   0        0        0     2042 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_child.py
+-rw-rw-rw-   0        0        0     2065 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_child_py3.py
+-rw-rw-rw-   0        0        0     1256 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_request.py
+-rw-rw-rw-   0        0        0     1265 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_request_py3.py
+-rw-rw-rw-   0        0        0     2593 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_hierarchy_response.py
+-rw-rw-rw-   0        0        0     2643 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_hierarchy_response_py3.py
+-rw-rw-rw-   0        0        0     1358 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_request.py
+-rw-rw-rw-   0        0        0     1368 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_request_py3.py
+-rw-rw-rw-   0        0        0     1224 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_response.py
+-rw-rw-rw-   0        0        0     1226 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_response_py3.py
+-rw-rw-rw-   0        0        0     1708 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_request.py
+-rw-rw-rw-   0        0        0     1711 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_request_py3.py
+-rw-rw-rw-   0        0        0     3015 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_response.py
+-rw-rw-rw-   0        0        0     3150 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_response_py3.py
+-rw-rw-rw-   0        0        0     1779 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_child.py
+-rw-rw-rw-   0        0        0     1830 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_child_py3.py
+-rw-rw-rw-   0        0        0     2066 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_response.py
+-rw-rw-rw-   0        0        0     2096 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_response_py3.py
+-rw-rw-rw-   0        0        0     1760 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_meter.py
+-rw-rw-rw-   0        0        0     1775 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_meter_py3.py
+-rw-rw-rw-   0        0        0     2426 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_property.py
+-rw-rw-rw-   0        0        0     2468 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_property_py3.py
+-rw-rw-rw-   0        0        0     1502 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_rating_child.py
+-rw-rw-rw-   0        0        0     1535 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_rating_child_py3.py
+-rw-rw-rw-   0        0        0     1506 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_request.py
+-rw-rw-rw-   0        0        0     1534 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_request_py3.py
+-rw-rw-rw-   0        0        0     3612 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_response.py
+-rw-rw-rw-   0        0        0     3791 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_response_py3.py
+-rw-rw-rw-   0        0        0     1417 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_place_child.py
+-rw-rw-rw-   0        0        0     1423 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_place_child_py3.py
+-rw-rw-rw-   0        0        0     1187 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_request.py
+-rw-rw-rw-   0        0        0     1186 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_request_py3.py
+-rw-rw-rw-   0        0        0     1040 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_place_child.py
+-rw-rw-rw-   0        0        0     1045 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_place_child_py3.py
+-rw-rw-rw-   0        0        0     3549 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_response.py
+-rw-rw-rw-   0        0        0     3637 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_response_py3.py
+-rw-rw-rw-   0        0        0     1994 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_class_permission.py
+-rw-rw-rw-   0        0        0      879 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2042 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_py3.py
+-rw-rw-rw-   0        0        0      851 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/environment.py
+-rw-rw-rw-   0        0        0      858 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/environment_py3.py
+-rw-rw-rw-   0        0        0     1581 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/estimated.py
+-rw-rw-rw-   0        0        0     1588 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/estimated_py3.py
+-rw-rw-rw-   0        0        0     2096 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills.py
+-rw-rw-rw-   0        0        0      975 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_class_permission.py
+-rw-rw-rw-   0        0        0      978 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2141 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_py3.py
+-rw-rw-rw-   0        0        0      920 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_format_child.py
+-rw-rw-rw-   0        0        0      943 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_format_child_py3.py
+-rw-rw-rw-   0        0        0     1835 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold.py
+-rw-rw-rw-   0        0        0      714 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_class_permission.py
+-rw-rw-rw-   0        0        0      724 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1887 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_py3.py
+-rw-rw-rw-   0        0        0     1840 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_child.py
+-rw-rw-rw-   0        0        0     1855 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_child_py3.py
+-rw-rw-rw-   0        0        0      946 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_settings.py
+-rw-rw-rw-   0        0        0      971 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_settings_py3.py
+-rw-rw-rw-   0        0        0     2261 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects.py
+-rw-rw-rw-   0        0        0     1140 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_class_permission.py
+-rw-rw-rw-   0        0        0     1143 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2306 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_py3.py
+-rw-rw-rw-   0        0        0     2119 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_reading_response.py
+-rw-rw-rw-   0        0        0     2173 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_reading_response_py3.py
+-rw-rw-rw-   0        0        0     1245 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_readings.py
+-rw-rw-rw-   0        0        0     1241 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_readings_py3.py
+-rw-rw-rw-   0        0        0     1850 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/file_data_type_response.py
+-rw-rw-rw-   0        0        0     1908 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/file_data_type_response_py3.py
+-rw-rw-rw-   0        0        0      685 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_data_response.py
+-rw-rw-rw-   0        0        0      693 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_data_response_py3.py
+-rw-rw-rw-   0        0        0     1371 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_edit.py
+-rw-rw-rw-   0        0        0     1369 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_edit_py3.py
+-rw-rw-rw-   0        0        0     3278 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_response.py
+-rw-rw-rw-   0        0        0     3307 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_response_py3.py
+-rw-rw-rw-   0        0        0      910 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_amount_response.py
+-rw-rw-rw-   0        0        0      912 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_amount_response_py3.py
+-rw-rw-rw-   0        0        0     1342 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_demand_request.py
+-rw-rw-rw-   0        0        0     1355 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_demand_request_py3.py
+-rw-rw-rw-   0        0        0     2080 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage.py
+-rw-rw-rw-   0        0        0     2112 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_py3.py
+-rw-rw-rw-   0        0        0     1628 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_response.py
+-rw-rw-rw-   0        0        0     1663 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_response_py3.py
+-rw-rw-rw-   0        0        0     1312 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_unit_cost_request.py
+-rw-rw-rw-   0        0        0     1315 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_unit_cost_request_py3.py
+-rw-rw-rw-   0        0        0     1306 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_use_request.py
+-rw-rw-rw-   0        0        0     1316 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_use_request_py3.py
+-rw-rw-rw-   0        0        0      979 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_action_child.py
+-rw-rw-rw-   0        0        0     1004 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_action_child_py3.py
+-rw-rw-rw-   0        0        0     2886 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_edit.py
+-rw-rw-rw-   0        0        0     2930 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_edit_py3.py
+-rw-rw-rw-   0        0        0     1765 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_event_child.py
+-rw-rw-rw-   0        0        0     1777 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_event_child_py3.py
+-rw-rw-rw-   0        0        0     1587 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_issue_type_child.py
+-rw-rw-rw-   0        0        0     1650 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_issue_type_child_py3.py
+-rw-rw-rw-   0        0        0      999 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_list_action.py
+-rw-rw-rw-   0        0        0     1005 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_list_action_py3.py
+-rw-rw-rw-   0        0        0     3186 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_response.py
+-rw-rw-rw-   0        0        0     3183 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_response_py3.py
+-rw-rw-rw-   0        0        0      979 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_status_child.py
+-rw-rw-rw-   0        0        0     1004 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_status_child_py3.py
+-rw-rw-rw-   0        0        0      945 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_child.py
+-rw-rw-rw-   0        0        0      966 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_child_py3.py
+-rw-rw-rw-   0        0        0     1090 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_create.py
+-rw-rw-rw-   0        0        0     1102 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_create_py3.py
+-rw-rw-rw-   0        0        0     2519 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget.py
+-rw-rw-rw-   0        0        0     3784 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_child.py
+-rw-rw-rw-   0        0        0     3832 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_child_py3.py
+-rw-rw-rw-   0        0        0     2560 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_py3.py
+-rw-rw-rw-   0        0        0     1973 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items.py
+-rw-rw-rw-   0        0        0      852 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_class_permission.py
+-rw-rw-rw-   0        0        0      859 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_py3.py
+-rw-rw-rw-   0        0        0     2265 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split.py
+-rw-rw-rw-   0        0        0     2297 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_py3.py
+-rw-rw-rw-   0        0        0     1913 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_response.py
+-rw-rw-rw-   0        0        0     1958 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_response_py3.py
+-rw-rw-rw-   0        0        0     1463 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_child.py
+-rw-rw-rw-   0        0        0     1474 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_child_py3.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_request.py
+-rw-rw-rw-   0        0        0     1406 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_request_py3.py
+-rw-rw-rw-   0        0        0     1893 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_response.py
+-rw-rw-rw-   0        0        0     1904 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_response_py3.py
+-rw-rw-rw-   0        0        0     2209 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/frequency.py
+-rw-rw-rw-   0        0        0     2269 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/frequency_py3.py
+-rw-rw-rw-   0        0        0     1191 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_child.py
+-rw-rw-rw-   0        0        0     1233 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_child_py3.py
+-rw-rw-rw-   0        0        0     1513 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_request.py
+-rw-rw-rw-   0        0        0     1521 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_request_py3.py
+-rw-rw-rw-   0        0        0     1308 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_response.py
+-rw-rw-rw-   0        0        0     1335 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_response_py3.py
+-rw-rw-rw-   0        0        0     2281 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_request.py
+-rw-rw-rw-   0        0        0     2309 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_request_py3.py
+-rw-rw-rw-   0        0        0     1515 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_response.py
+-rw-rw-rw-   0        0        0     1535 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_response_py3.py
+-rw-rw-rw-   0        0        0      896 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_count.py
+-rw-rw-rw-   0        0        0      907 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_count_py3.py
+-rw-rw-rw-   0        0        0     3365 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_building_rank.py
+-rw-rw-rw-   0        0        0     3411 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_building_rank_py3.py
+-rw-rw-rw-   0        0        0     1310 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_carbon_footprint_response.py
+-rw-rw-rw-   0        0        0     1316 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_carbon_footprint_response_py3.py
+-rw-rw-rw-   0        0        0     1423 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_factor.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_factor_py3.py
+-rw-rw-rw-   0        0        0     1375 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_request.py
+-rw-rw-rw-   0        0        0     1400 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_request_py3.py
+-rw-rw-rw-   0        0        0     1953 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_response.py
+-rw-rw-rw-   0        0        0     1999 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1638 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor.py
+-rw-rw-rw-   0        0        0     1375 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_by_category_child.py
+-rw-rw-rw-   0        0        0     1396 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_by_category_child_py3.py
+-rw-rw-rw-   0        0        0     1038 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category.py
+-rw-rw-rw-   0        0        0     1071 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_py3.py
+-rw-rw-rw-   0        0        0     1317 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_response.py
+-rw-rw-rw-   0        0        0     1344 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_response_py3.py
+-rw-rw-rw-   0        0        0     1668 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_py3.py
+-rw-rw-rw-   0        0        0     2528 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_version_history_response.py
+-rw-rw-rw-   0        0        0     2548 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_version_history_response_py3.py
+-rw-rw-rw-   0        0        0     2657 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factors_response.py
+-rw-rw-rw-   0        0        0     2663 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factors_response_py3.py
+-rw-rw-rw-   0        0        0     1196 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_gas.py
+-rw-rw-rw-   0        0        0     1213 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_gas_py3.py
+-rw-rw-rw-   0        0        0     1008 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_group_emissions.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_group_emissions_py3.py
+-rw-rw-rw-   0        0        0     3413 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_performance_comparison.py
+-rw-rw-rw-   0        0        0     3491 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_performance_comparison_py3.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope.py
+-rw-rw-rw-   0        0        0     1492 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category.py
+-rw-rw-rw-   0        0        0     1339 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_child.py
+-rw-rw-rw-   0        0        0     1388 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_child_py3.py
+-rw-rw-rw-   0        0        0     1533 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_py3.py
+-rw-rw-rw-   0        0        0      886 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_py3.py
+-rw-rw-rw-   0        0        0     1210 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_response.py
+-rw-rw-rw-   0        0        0     1226 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_response_py3.py
+-rw-rw-rw-   0        0        0     1280 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_request.py
+-rw-rw-rw-   0        0        0     1291 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_request_py3.py
+-rw-rw-rw-   0        0        0     1866 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_response.py
+-rw-rw-rw-   0        0        0     1886 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1505 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_settings.py
+-rw-rw-rw-   0        0        0     1573 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_settings_py3.py
+-rw-rw-rw-   0        0        0     1376 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_target_emissions.py
+-rw-rw-rw-   0        0        0     1408 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_target_emissions_py3.py
+-rw-rw-rw-   0        0        0     1133 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_type_child.py
+-rw-rw-rw-   0        0        0     1157 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_type_child_py3.py
+-rw-rw-rw-   0        0        0     1087 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_version.py
+-rw-rw-rw-   0        0        0     1089 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_version_py3.py
+-rw-rw-rw-   0        0        0     2361 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_yearly_emissions.py
+-rw-rw-rw-   0        0        0     2434 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_yearly_emissions_py3.py
+-rw-rw-rw-   0        0        0     1129 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child.py
+-rw-rw-rw-   0        0        0     1148 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_py3.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_request.py
+-rw-rw-rw-   0        0        0     1386 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_request_py3.py
+-rw-rw-rw-   0        0        0     2276 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_request.py
+-rw-rw-rw-   0        0        0     2290 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_request_py3.py
+-rw-rw-rw-   0        0        0     1497 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_response.py
+-rw-rw-rw-   0        0        0     1526 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_response_py3.py
+-rw-rw-rw-   0        0        0     2018 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings.py
+-rw-rw-rw-   0        0        0      897 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_class_permission.py
+-rw-rw-rw-   0        0        0      904 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2067 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator.py
+-rw-rw-rw-   0        0        0      762 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_class_permission.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1935 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_py3.py
+-rw-rw-rw-   0        0        0     3079 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_display_setting.py
+-rw-rw-rw-   0        0        0     3167 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_display_setting_py3.py
+-rw-rw-rw-   0        0        0     1043 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_member_request.py
+-rw-rw-rw-   0        0        0     1059 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_member_request_py3.py
+-rw-rw-rw-   0        0        0     4100 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_meter_group_response.py
+-rw-rw-rw-   0        0        0     4227 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_meter_group_response_py3.py
+-rw-rw-rw-   0        0        0     2017 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_member.py
+-rw-rw-rw-   0        0        0     2032 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_member_py3.py
+-rw-rw-rw-   0        0        0     3601 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_response.py
+-rw-rw-rw-   0        0        0     3715 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_response_py3.py
+-rw-rw-rw-   0        0        0     1868 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module.py
+-rw-rw-rw-   0        0        0      747 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_class_permission.py
+-rw-rw-rw-   0        0        0      755 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1918 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_py3.py
+-rw-rw-rw-   0        0        0      735 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/guid_response.py
+-rw-rw-rw-   0        0        0      748 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/guid_response_py3.py
+-rw-rw-rw-   0        0        0      989 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hidden_request.py
+-rw-rw-rw-   0        0        0      994 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hidden_request_py3.py
+-rw-rw-rw-   0        0        0     3463 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers.py
+-rw-rw-rw-   0        0        0     3023 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers2.py
+-rw-rw-rw-   0        0        0     3134 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers2_py3.py
+-rw-rw-rw-   0        0        0     3574 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers_py3.py
+-rw-rw-rw-   0        0        0     3310 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places.py
+-rw-rw-rw-   0        0        0     2940 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places2.py
+-rw-rw-rw-   0        0        0     3020 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places2_py3.py
+-rw-rw-rw-   0        0        0     3390 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places_py3.py
+-rw-rw-rw-   0        0        0     1841 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data.py
+-rw-rw-rw-   0        0        0     1853 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis.py
+-rw-rw-rw-   0        0        0      732 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_class_permission.py
+-rw-rw-rw-   0        0        0      740 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1903 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_py3.py
+-rw-rw-rw-   0        0        0      720 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_class_permission.py
+-rw-rw-rw-   0        0        0      730 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1893 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_py3.py
+-rw-rw-rw-   0        0        0     1841 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup.py
+-rw-rw-rw-   0        0        0      720 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_class_permission.py
+-rw-rw-rw-   0        0        0      727 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1890 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_py3.py
+-rw-rw-rw-   0        0        0     1381 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_response.py
+-rw-rw-rw-   0        0        0     1389 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_response_py3.py
+-rw-rw-rw-   0        0        0     1604 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_with_unit_response.py
+-rw-rw-rw-   0        0        0     1609 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_with_unit_response_py3.py
+-rw-rw-rw-   0        0        0     1533 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/latest_benchmark_value.py
+-rw-rw-rw-   0        0        0     1568 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/latest_benchmark_value_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accounting_export.py
+-rw-rw-rw-   0        0        0     1933 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accounting_export_py3.py
+-rw-rw-rw-   0        0        0     1871 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accrual_bills.py
+-rw-rw-rw-   0        0        0     1921 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accrual_bills_py3.py
+-rw-rw-rw-   0        0        0     1868 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_chargebacks.py
+-rw-rw-rw-   0        0        0     1918 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_chargebacks_py3.py
+-rw-rw-rw-   0        0        0     1874 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_cost_avoidance.py
+-rw-rw-rw-   0        0        0     1924 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_cost_avoidance_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_custom_benchmarks.py
+-rw-rw-rw-   0        0        0     1933 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_custom_benchmarks_py3.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_ghg.py
+-rw-rw-rw-   0        0        0     1894 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_ghg_py3.py
+-rw-rw-rw-   0        0        0     1895 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_interval_data_analysis.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_interval_data_analysis_py3.py
+-rw-rw-rw-   0        0        0     1877 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_designer.py
+-rw-rw-rw-   0        0        0     1927 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_designer_py3.py
+-rw-rw-rw-   0        0        0     1889 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_distribution.py
+-rw-rw-rw-   0        0        0     1939 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_distribution_py3.py
+-rw-rw-rw-   0        0        0     2873 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_features.py
+-rw-rw-rw-   0        0        0     2952 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_features_py3.py
+-rw-rw-rw-   0        0        0      820 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_request.py
+-rw-rw-rw-   0        0        0      837 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_request_py3.py
+-rw-rw-rw-   0        0        0     3076 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_response.py
+-rw-rw-rw-   0        0        0     3128 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_response_py3.py
+-rw-rw-rw-   0        0        0     1011 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_accrual_exclusion.py
+-rw-rw-rw-   0        0        0     1017 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_accrual_exclusion_py3.py
+-rw-rw-rw-   0        0        0      755 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_approve.py
+-rw-rw-rw-   0        0        0      766 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_approve_py3.py
+-rw-rw-rw-   0        0        0      976 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_custom.py
+-rw-rw-rw-   0        0        0      984 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_custom_py3.py
+-rw-rw-rw-   0        0        0      792 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_export_hold.py
+-rw-rw-rw-   0        0        0      807 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_export_hold_py3.py
+-rw-rw-rw-   0        0        0      773 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_reverse.py
+-rw-rw-rw-   0        0        0      785 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_reverse_py3.py
+-rw-rw-rw-   0        0        0      728 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_void.py
+-rw-rw-rw-   0        0        0      736 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_void_py3.py
+-rw-rw-rw-   0        0        0     2432 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_column_edit.py
+-rw-rw-rw-   0        0        0     2423 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_column_edit_py3.py
+-rw-rw-rw-   0        0        0     1381 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_copy.py
+-rw-rw-rw-   0        0        0     1396 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_copy_py3.py
+-rw-rw-rw-   0        0        0     1694 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create.py
+-rw-rw-rw-   0        0        0     1708 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_py3.py
+-rw-rw-rw-   0        0        0     1865 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_response.py
+-rw-rw-rw-   0        0        0     1875 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_response_py3.py
+-rw-rw-rw-   0        0        0     1444 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_edit.py
+-rw-rw-rw-   0        0        0     1459 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_edit_py3.py
+-rw-rw-rw-   0        0        0      707 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_ids.py
+-rw-rw-rw-   0        0        0      708 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_ids_py3.py
+-rw-rw-rw-   0        0        0     1597 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response.py
+-rw-rw-rw-   0        0        0     2495 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_field.py
+-rw-rw-rw-   0        0        0     2530 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_field_py3.py
+-rw-rw-rw-   0        0        0      980 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_item.py
+-rw-rw-rw-   0        0        0      979 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_item_py3.py
+-rw-rw-rw-   0        0        0     1581 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_py3.py
+-rw-rw-rw-   0        0        0     1128 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_type_child.py
+-rw-rw-rw-   0        0        0     1162 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_type_child_py3.py
+-rw-rw-rw-   0        0        0     1767 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_request.py
+-rw-rw-rw-   0        0        0     1767 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_request_py3.py
+-rw-rw-rw-   0        0        0      830 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_response.py
+-rw-rw-rw-   0        0        0      829 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_response_py3.py
+-rw-rw-rw-   0        0        0     2330 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manual_adjustment_request.py
+-rw-rw-rw-   0        0        0     2349 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manual_adjustment_request_py3.py
+-rw-rw-rw-   0        0        0     2000 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings.py
+-rw-rw-rw-   0        0        0      879 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_class_permission.py
+-rw-rw-rw-   0        0        0      886 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2049 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_py3.py
+-rw-rw-rw-   0        0        0     3776 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_request.py
+-rw-rw-rw-   0        0        0     3815 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_request_py3.py
+-rw-rw-rw-   0        0        0     2985 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_response.py
+-rw-rw-rw-   0        0        0     3028 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_response_py3.py
+-rw-rw-rw-   0        0        0     2526 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_place_child.py
+-rw-rw-rw-   0        0        0     2573 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_place_child_py3.py
+-rw-rw-rw-   0        0        0     2254 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_widget_response.py
+-rw-rw-rw-   0        0        0     2296 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_widget_response_py3.py
+-rw-rw-rw-   0        0        0    10112 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/me.py
+-rw-rw-rw-   0        0        0    10371 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_py3.py
+-rw-rw-rw-   0        0        0     1303 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_request.py
+-rw-rw-rw-   0        0        0     1309 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_request_py3.py
+-rw-rw-rw-   0        0        0      943 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/message.py
+-rw-rw-rw-   0        0        0      957 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/message_py3.py
+-rw-rw-rw-   0        0        0     4342 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_account_child.py
+-rw-rw-rw-   0        0        0     4425 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_account_child_py3.py
+-rw-rw-rw-   0        0        0    13718 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_bill_response.py
+-rw-rw-rw-   0        0        0    13849 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_bill_response_py3.py
+-rw-rw-rw-   0        0        0     3166 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_calendarized_use_vs_weather_response.py
+-rw-rw-rw-   0        0        0     3302 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_calendarized_use_vs_weather_response_py3.py
+-rw-rw-rw-   0        0        0     1245 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cap_response.py
+-rw-rw-rw-   0        0        0     1259 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cap_response_py3.py
+-rw-rw-rw-   0        0        0     1680 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_request.py
+-rw-rw-rw-   0        0        0     1715 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_request_py3.py
+-rw-rw-rw-   0        0        0     2239 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_response.py
+-rw-rw-rw-   0        0        0     2339 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_response_py3.py
+-rw-rw-rw-   0        0        0     2713 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child.py
+-rw-rw-rw-   0        0        0     3237 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_meter_import_id_and_route.py
+-rw-rw-rw-   0        0        0     3287 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_meter_import_id_and_route_py3.py
+-rw-rw-rw-   0        0        0     3059 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_and_serial_number.py
+-rw-rw-rw-   0        0        0     3109 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_and_serial_number_py3.py
+-rw-rw-rw-   0        0        0     3342 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_channel_latest_reading.py
+-rw-rw-rw-   0        0        0     3387 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_channel_latest_reading_py3.py
+-rw-rw-rw-   0        0        0     2764 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_py3.py
+-rw-rw-rw-   0        0        0     3337 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_search.py
+-rw-rw-rw-   0        0        0     3402 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_search_py3.py
+-rw-rw-rw-   0        0        0     1239 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cost.py
+-rw-rw-rw-   0        0        0     1234 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cost_py3.py
+-rw-rw-rw-   0        0        0     5449 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_create.py
+-rw-rw-rw-   0        0        0     5490 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_create_py3.py
+-rw-rw-rw-   0        0        0     2572 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response.py
+-rw-rw-rw-   0        0        0     2580 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     4151 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results.py
+-rw-rw-rw-   0        0        0     4302 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2566 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response.py
+-rw-rw-rw-   0        0        0     2574 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     2295 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results.py
+-rw-rw-rw-   0        0        0     2366 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2517 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response.py
+-rw-rw-rw-   0        0        0     2525 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_py3.py
+-rw-rw-rw-   0        0        0     4398 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_results.py
+-rw-rw-rw-   0        0        0     4566 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_results_py3.py
+-rw-rw-rw-   0        0        0     2179 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response.py
+-rw-rw-rw-   0        0        0     1680 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope.py
+-rw-rw-rw-   0        0        0     1729 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope_py3.py
+-rw-rw-rw-   0        0        0     1453 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type.py
+-rw-rw-rw-   0        0        0     1471 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type_py3.py
+-rw-rw-rw-   0        0        0     2196 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1012 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1037 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2324 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response.py
+-rw-rw-rw-   0        0        0     2336 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     3068 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_results.py
+-rw-rw-rw-   0        0        0     3154 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2318 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response.py
+-rw-rw-rw-   0        0        0     2330 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1317 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1339 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2463 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response.py
+-rw-rw-rw-   0        0        0     2462 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     3409 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_results.py
+-rw-rw-rw-   0        0        0     3503 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     5516 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response.py
+-rw-rw-rw-   0        0        0     5679 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     2883 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_results.py
+-rw-rw-rw-   0        0        0     2968 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     6184 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_edit.py
+-rw-rw-rw-   0        0        0     6219 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_edit_py3.py
+-rw-rw-rw-   0        0        0     1311 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_category_child.py
+-rw-rw-rw-   0        0        0     1371 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_category_child_py3.py
+-rw-rw-rw-   0        0        0     1718 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_child.py
+-rw-rw-rw-   0        0        0     1770 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_child_py3.py
+-rw-rw-rw-   0        0        0     2660 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_child.py
+-rw-rw-rw-   0        0        0     2724 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_child_py3.py
+-rw-rw-rw-   0        0        0     2973 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_child.py
+-rw-rw-rw-   0        0        0     3034 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_child_py3.py
+-rw-rw-rw-   0        0        0     4066 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_response.py
+-rw-rw-rw-   0        0        0     4161 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_response_py3.py
+-rw-rw-rw-   0        0        0     3599 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_child.py
+-rw-rw-rw-   0        0        0     3669 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_child_py3.py
+-rw-rw-rw-   0        0        0     5914 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_response.py
+-rw-rw-rw-   0        0        0     6070 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_response_py3.py
+-rw-rw-rw-   0        0        0     1169 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member.py
+-rw-rw-rw-   0        0        0     3470 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_child.py
+-rw-rw-rw-   0        0        0     3518 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_child_py3.py
+-rw-rw-rw-   0        0        0     1196 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_py3.py
+-rw-rw-rw-   0        0        0     2959 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_request.py
+-rw-rw-rw-   0        0        0     3012 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_request_py3.py
+-rw-rw-rw-   0        0        0     2277 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_response.py
+-rw-rw-rw-   0        0        0     2335 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_response_py3.py
+-rw-rw-rw-   0        0        0     2020 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_rate_response.py
+-rw-rw-rw-   0        0        0     2005 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_rate_response_py3.py
+-rw-rw-rw-   0        0        0     7316 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_response.py
+-rw-rw-rw-   0        0        0     7381 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_response_py3.py
+-rw-rw-rw-   0        0        0     1997 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings.py
+-rw-rw-rw-   0        0        0      876 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_class_permission.py
+-rw-rw-rw-   0        0        0      883 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2046 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_py3.py
+-rw-rw-rw-   0        0        0     1626 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_search_request.py
+-rw-rw-rw-   0        0        0     1637 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_search_request_py3.py
+-rw-rw-rw-   0        0        0     1149 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_child.py
+-rw-rw-rw-   0        0        0     1186 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_child_py3.py
+-rw-rw-rw-   0        0        0     1531 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_request.py
+-rw-rw-rw-   0        0        0     1558 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_request_py3.py
+-rw-rw-rw-   0        0        0     1406 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_response.py
+-rw-rw-rw-   0        0        0     1430 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_response_py3.py
+-rw-rw-rw-   0        0        0     1839 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_template_response.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_template_response_py3.py
+-rw-rw-rw-   0        0        0     1107 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_type_child.py
+-rw-rw-rw-   0        0        0     1137 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_type_child_py3.py
+-rw-rw-rw-   0        0        0     1296 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_udf_response.py
+-rw-rw-rw-   0        0        0     1302 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_udf_response_py3.py
+-rw-rw-rw-   0        0        0     2231 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters.py
+-rw-rw-rw-   0        0        0     1110 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_class_permission.py
+-rw-rw-rw-   0        0        0     1113 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2276 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_py3.py
+-rw-rw-rw-   0        0        0     1839 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/missing_bill_widget.py
+-rw-rw-rw-   0        0        0     1858 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/missing_bill_widget_py3.py
+-rw-rw-rw-   0        0        0     1706 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/monthly_cap_trend.py
+-rw-rw-rw-   0        0        0     1747 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/monthly_cap_trend_py3.py
+-rw-rw-rw-   0        0        0     1039 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/most_recent_aggregate.py
+-rw-rw-rw-   0        0        0     1061 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/most_recent_aggregate_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors.py
+-rw-rw-rw-   0        0        0      762 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_class_permission.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1935 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_py3.py
+-rw-rw-rw-   0        0        0     1137 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_bills_destination.py
+-rw-rw-rw-   0        0        0     1141 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_bills_destination_py3.py
+-rw-rw-rw-   0        0        0     1337 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_create_meter.py
+-rw-rw-rw-   0        0        0     1356 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_create_meter_py3.py
+-rw-rw-rw-   0        0        0     1856 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills.py
+-rw-rw-rw-   0        0        0      735 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_class_permission.py
+-rw-rw-rw-   0        0        0      745 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1908 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_py3.py
+-rw-rw-rw-   0        0        0     1156 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/named_period.py
+-rw-rw-rw-   0        0        0     1168 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/named_period_py3.py
+-rw-rw-rw-   0        0        0     2000 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings.py
+-rw-rw-rw-   0        0        0      879 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_class_permission.py
+-rw-rw-rw-   0        0        0      886 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2049 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_py3.py
+-rw-rw-rw-   0        0        0     1177 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_action_button_response.py
+-rw-rw-rw-   0        0        0     1191 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_action_button_response_py3.py
+-rw-rw-rw-   0        0        0     1450 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_badge_response.py
+-rw-rw-rw-   0        0        0     1492 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_badge_response_py3.py
+-rw-rw-rw-   0        0        0     1480 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_category.py
+-rw-rw-rw-   0        0        0     1550 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_category_py3.py
+-rw-rw-rw-   0        0        0     2803 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_details_response.py
+-rw-rw-rw-   0        0        0     2826 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_details_response_py3.py
+-rw-rw-rw-   0        0        0     2073 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_response.py
+-rw-rw-rw-   0        0        0     2098 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_response_py3.py
+-rw-rw-rw-   0        0        0     1848 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_request.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_request_py3.py
+-rw-rw-rw-   0        0        0     1513 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_response.py
+-rw-rw-rw-   0        0        0     1567 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1328 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_settings_response.py
+-rw-rw-rw-   0        0        0     1374 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_settings_response_py3.py
+-rw-rw-rw-   0        0        0     1711 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_system_settings_request.py
+-rw-rw-rw-   0        0        0     1752 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_system_settings_request_py3.py
+-rw-rw-rw-   0        0        0     1671 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_type.py
+-rw-rw-rw-   0        0        0     1737 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_type_py3.py
+-rw-rw-rw-   0        0        0     1643 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_update_request.py
+-rw-rw-rw-   0        0        0     1650 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_update_request_py3.py
+-rw-rw-rw-   0        0        0     1423 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_method_child.py
+-rw-rw-rw-   0        0        0     1477 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_method_child_py3.py
+-rw-rw-rw-   0        0        0     1302 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_rule.py
+-rw-rw-rw-   0        0        0     1350 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_rule_py3.py
+-rw-rw-rw-   0        0        0     2143 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type.py
+-rw-rw-rw-   0        0        0     1964 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child.py
+-rw-rw-rw-   0        0        0     1329 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_base.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_base_py3.py
+-rw-rw-rw-   0        0        0     2010 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_py3.py
+-rw-rw-rw-   0        0        0     2188 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_py3.py
+-rw-rw-rw-   0        0        0     1719 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_object_result.py
+-rw-rw-rw-   0        0        0     1727 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_object_result_py3.py
+-rw-rw-rw-   0        0        0      690 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_result.py
+-rw-rw-rw-   0        0        0      704 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_result_py3.py
+-rw-rw-rw-   0        0        0     1135 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category.py
+-rw-rw-rw-   0        0        0     1182 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_py3.py
+-rw-rw-rw-   0        0        0      869 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_request.py
+-rw-rw-rw-   0        0        0      899 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_request_py3.py
+-rw-rw-rw-   0        0        0     3459 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_request.py
+-rw-rw-rw-   0        0        0     3501 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_request_py3.py
+-rw-rw-rw-   0        0        0     3759 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_response.py
+-rw-rw-rw-   0        0        0     3817 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_response_py3.py
+-rw-rw-rw-   0        0        0     1566 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/outlier_severity_child.py
+-rw-rw-rw-   0        0        0     1598 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/outlier_severity_child_py3.py
+-rw-rw-rw-   0        0        0     1485 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_comparison.py
+-rw-rw-rw-   0        0        0     1510 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_comparison_py3.py
+-rw-rw-rw-   0        0        0      951 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range.py
+-rw-rw-rw-   0        0        0     1110 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison.py
+-rw-rw-rw-   0        0        0     1818 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_detailed.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_detailed_py3.py
+-rw-rw-rw-   0        0        0     1136 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_py3.py
+-rw-rw-rw-   0        0        0      968 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_py3.py
+-rw-rw-rw-   0        0        0     1103 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_value.py
+-rw-rw-rw-   0        0        0     1118 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_value_py3.py
+-rw-rw-rw-   0        0        0    23430 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions.py
+-rw-rw-rw-   0        0        0    24140 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_py3.py
+-rw-rw-rw-   0        0        0    22391 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_request.py
+-rw-rw-rw-   0        0        0    22943 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_request_py3.py
+-rw-rw-rw-   0        0        0     1680 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_request.py
+-rw-rw-rw-   0        0        0     1715 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_request_py3.py
+-rw-rw-rw-   0        0        0     2239 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_response.py
+-rw-rw-rw-   0        0        0     2339 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_response_py3.py
+-rw-rw-rw-   0        0        0     1274 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child.py
+-rw-rw-rw-   0        0        0     1286 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_py3.py
+-rw-rw-rw-   0        0        0     1587 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_with_floor_area.py
+-rw-rw-rw-   0        0        0     1604 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_with_floor_area_py3.py
+-rw-rw-rw-   0        0        0     1852 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_cost.py
+-rw-rw-rw-   0        0        0     1876 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_cost_py3.py
+-rw-rw-rw-   0        0        0     3811 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_create.py
+-rw-rw-rw-   0        0        0     3836 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_create_py3.py
+-rw-rw-rw-   0        0        0     2969 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response.py
+-rw-rw-rw-   0        0        0     2594 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2622 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     3916 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     4059 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2971 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     2736 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results.py
+-rw-rw-rw-   0        0        0     2822 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2801 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response.py
+-rw-rw-rw-   0        0        0     2634 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2662 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     2322 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     2393 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2804 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1383 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1412 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2034 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison.py
+-rw-rw-rw-   0        0        0     2076 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison_py3.py
+-rw-rw-rw-   0        0        0     2007 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_comparison_response.py
+-rw-rw-rw-   0        0        0     2021 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_comparison_response_py3.py
+-rw-rw-rw-   0        0        0     2530 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity.py
+-rw-rw-rw-   0        0        0     1629 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity.py
+-rw-rw-rw-   0        0        0     1658 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity_py3.py
+-rw-rw-rw-   0        0        0     1598 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project.py
+-rw-rw-rw-   0        0        0     1651 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project_py3.py
+-rw-rw-rw-   0        0        0     2570 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_py3.py
+-rw-rw-rw-   0        0        0     2583 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response.py
+-rw-rw-rw-   0        0        0     1808 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity.py
+-rw-rw-rw-   0        0        0     1833 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity_py3.py
+-rw-rw-rw-   0        0        0     1801 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope.py
+-rw-rw-rw-   0        0        0     1826 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope_py3.py
+-rw-rw-rw-   0        0        0     1777 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type.py
+-rw-rw-rw-   0        0        0     1799 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type_py3.py
+-rw-rw-rw-   0        0        0     2599 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     1860 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_results.py
+-rw-rw-rw-   0        0        0     1912 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1277 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison.py
+-rw-rw-rw-   0        0        0     1289 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison_py3.py
+-rw-rw-rw-   0        0        0     2246 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response.py
+-rw-rw-rw-   0        0        0     1971 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope.py
+-rw-rw-rw-   0        0        0     2016 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope_py3.py
+-rw-rw-rw-   0        0        0     1769 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type.py
+-rw-rw-rw-   0        0        0     1791 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type_py3.py
+-rw-rw-rw-   0        0        0     2264 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1012 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1037 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1690 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison.py
+-rw-rw-rw-   0        0        0     1748 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison_py3.py
+-rw-rw-rw-   0        0        0     1362 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly.py
+-rw-rw-rw-   0        0        0     2499 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results.py
+-rw-rw-rw-   0        0        0     2563 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     1374 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_py3.py
+-rw-rw-rw-   0        0        0     2504 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response.py
+-rw-rw-rw-   0        0        0     2384 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2416 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     2448 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     2512 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2511 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     1784 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_results.py
+-rw-rw-rw-   0        0        0     1822 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1299 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly.py
+-rw-rw-rw-   0        0        0     1311 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_py3.py
+-rw-rw-rw-   0        0        0     1808 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results.py
+-rw-rw-rw-   0        0        0     1846 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results_py3.py
+-rw-rw-rw-   0        0        0     2509 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response.py
+-rw-rw-rw-   0        0        0     2118 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2145 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1143 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1158 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2516 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_py3.py
+-rw-rw-rw-   0        0        0      929 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_results.py
+-rw-rw-rw-   0        0        0      940 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1510 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison.py
+-rw-rw-rw-   0        0        0     1540 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison_py3.py
+-rw-rw-rw-   0        0        0     2374 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response.py
+-rw-rw-rw-   0        0        0     2005 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2366 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results.py
+-rw-rw-rw-   0        0        0     2436 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2024 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     2373 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_py3.py
+-rw-rw-rw-   0        0        0     2065 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_results.py
+-rw-rw-rw-   0        0        0     2123 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_results_py3.py
+-rw-rw-rw-   0        0        0     4245 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response.py
+-rw-rw-rw-   0        0        0     4797 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2948 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results.py
+-rw-rw-rw-   0        0        0     3033 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     4975 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     4350 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     2170 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_results.py
+-rw-rw-rw-   0        0        0     2229 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1249 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly.py
+-rw-rw-rw-   0        0        0     1261 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_py3.py
+-rw-rw-rw-   0        0        0     1778 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_results.py
+-rw-rw-rw-   0        0        0     1816 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_results_py3.py
+-rw-rw-rw-   0        0        0     4085 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_edit.py
+-rw-rw-rw-   0        0        0     4110 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_edit_py3.py
+-rw-rw-rw-   0        0        0     1311 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_category_child.py
+-rw-rw-rw-   0        0        0     1371 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_category_child_py3.py
+-rw-rw-rw-   0        0        0     1718 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_child.py
+-rw-rw-rw-   0        0        0     1770 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_child_py3.py
+-rw-rw-rw-   0        0        0     2600 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_child.py
+-rw-rw-rw-   0        0        0     2641 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_child_py3.py
+-rw-rw-rw-   0        0        0     6503 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_response.py
+-rw-rw-rw-   0        0        0     6630 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_response_py3.py
+-rw-rw-rw-   0        0        0     2199 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_child.py
+-rw-rw-rw-   0        0        0     2231 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_child_py3.py
+-rw-rw-rw-   0        0        0     5496 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_response.py
+-rw-rw-rw-   0        0        0     5591 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_response_py3.py
+-rw-rw-rw-   0        0        0     1432 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_child.py
+-rw-rw-rw-   0        0        0     1462 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_child_py3.py
+-rw-rw-rw-   0        0        0     1818 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_child.py
+-rw-rw-rw-   0        0        0     1857 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_child_py3.py
+-rw-rw-rw-   0        0        0     5090 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_response.py
+-rw-rw-rw-   0        0        0     5256 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_response_py3.py
+-rw-rw-rw-   0        0        0     1169 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_member.py
+-rw-rw-rw-   0        0        0     1196 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_member_py3.py
+-rw-rw-rw-   0        0        0     2959 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_request.py
+-rw-rw-rw-   0        0        0     3012 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_request_py3.py
+-rw-rw-rw-   0        0        0     2277 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_response.py
+-rw-rw-rw-   0        0        0     2335 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_response_py3.py
+-rw-rw-rw-   0        0        0     1056 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_info.py
+-rw-rw-rw-   0        0        0     1071 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_info_py3.py
+-rw-rw-rw-   0        0        0     5861 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_response.py
+-rw-rw-rw-   0        0        0     5838 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_response_py3.py
+-rw-rw-rw-   0        0        0     2127 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_child.py
+-rw-rw-rw-   0        0        0     2135 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_child_py3.py
+-rw-rw-rw-   0        0        0     2196 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_create.py
+-rw-rw-rw-   0        0        0     2192 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_create_py3.py
+-rw-rw-rw-   0        0        0     1278 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_submission_type_request.py
+-rw-rw-rw-   0        0        0     1292 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_submission_type_request_py3.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_request.py
+-rw-rw-rw-   0        0        0     1043 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_request_py3.py
+-rw-rw-rw-   0        0        0     1382 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_response.py
+-rw-rw-rw-   0        0        0     1414 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_response_py3.py
+-rw-rw-rw-   0        0        0     1296 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_udf_response.py
+-rw-rw-rw-   0        0        0     1302 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_udf_response_py3.py
+-rw-rw-rw-   0        0        0     1034 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/pm_commodity_child.py
+-rw-rw-rw-   0        0        0     1057 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/pm_commodity_child_py3.py
+-rw-rw-rw-   0        0        0     1518 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response.py
+-rw-rw-rw-   0        0        0     1526 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_py3.py
+-rw-rw-rw-   0        0        0     1796 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_weather_station.py
+-rw-rw-rw-   0        0        0     1827 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_weather_station_py3.py
+-rw-rw-rw-   0        0        0     6804 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference.py
+-rw-rw-rw-   0        0        0     7093 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_py3.py
+-rw-rw-rw-   0        0        0     7718 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_request.py
+-rw-rw-rw-   0        0        0     7996 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_request_py3.py
+-rw-rw-rw-   0        0        0     1128 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_child.py
+-rw-rw-rw-   0        0        0     1161 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_child_py3.py
+-rw-rw-rw-   0        0        0     1985 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_create.py
+-rw-rw-rw-   0        0        0     2005 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_create_py3.py
+-rw-rw-rw-   0        0        0     1337 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_response.py
+-rw-rw-rw-   0        0        0     1378 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_response_py3.py
+-rw-rw-rw-   0        0        0     1100 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/project_manager_response.py
+-rw-rw-rw-   0        0        0     1140 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/project_manager_response_py3.py
+-rw-rw-rw-   0        0        0     1871 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps.py
+-rw-rw-rw-   0        0        0      750 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_class_permission.py
+-rw-rw-rw-   0        0        0      760 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1923 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_py3.py
+-rw-rw-rw-   0        0        0     1365 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_filter.py
+-rw-rw-rw-   0        0        0     1357 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_filter_py3.py
+-rw-rw-rw-   0        0        0     1574 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_report.py
+-rw-rw-rw-   0        0        0     1581 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_report_py3.py
+-rw-rw-rw-   0        0        0      799 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child.py
+-rw-rw-rw-   0        0        0      805 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_py3.py
+-rw-rw-rw-   0        0        0     1027 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_response.py
+-rw-rw-rw-   0        0        0     1029 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_response_py3.py
+-rw-rw-rw-   0        0        0     1788 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_create.py
+-rw-rw-rw-   0        0        0     1781 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_create_py3.py
+-rw-rw-rw-   0        0        0     2114 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response.py
+-rw-rw-rw-   0        0        0     1956 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     1975 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1804 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1851 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2104 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1349 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1378 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1204 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_edit.py
+-rw-rw-rw-   0        0        0     1207 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_edit_py3.py
+-rw-rw-rw-   0        0        0     1530 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_response.py
+-rw-rw-rw-   0        0        0     1516 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_response_py3.py
+-rw-rw-rw-   0        0        0     2120 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules.py
+-rw-rw-rw-   0        0        0      999 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_class_permission.py
+-rw-rw-rw-   0        0        0     1005 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2168 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_py3.py
+-rw-rw-rw-   0        0        0     3957 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_request.py
+-rw-rw-rw-   0        0        0     3985 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_request_py3.py
+-rw-rw-rw-   0        0        0     3982 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_response.py
+-rw-rw-rw-   0        0        0     3982 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_response_py3.py
+-rw-rw-rw-   0        0        0     1744 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading.py
+-rw-rw-rw-   0        0        0     1464 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_child_base.py
+-rw-rw-rw-   0        0        0     1469 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_child_base_py3.py
+-rw-rw-rw-   0        0        0     4330 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_create.py
+-rw-rw-rw-   0        0        0     4382 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_create_py3.py
+-rw-rw-rw-   0        0        0     1627 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_delete.py
+-rw-rw-rw-   0        0        0     1627 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_delete_py3.py
+-rw-rw-rw-   0        0        0     6736 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile.py
+-rw-rw-rw-   0        0        0     1932 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_column.py
+-rw-rw-rw-   0        0        0     1952 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_column_py3.py
+-rw-rw-rw-   0        0        0     6876 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_py3.py
+-rw-rw-rw-   0        0        0     7173 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_request.py
+-rw-rw-rw-   0        0        0     7312 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_request_py3.py
+-rw-rw-rw-   0        0        0     5583 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_response.py
+-rw-rw-rw-   0        0        0     5733 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_response_py3.py
+-rw-rw-rw-   0        0        0     1829 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_request.py
+-rw-rw-rw-   0        0        0     1852 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_request_py3.py
+-rw-rw-rw-   0        0        0     1733 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_py3.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_response.py
+-rw-rw-rw-   0        0        0     1446 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_response_py3.py
+-rw-rw-rw-   0        0        0     1260 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings.py
+-rw-rw-rw-   0        0        0     2101 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_observation.py
+-rw-rw-rw-   0        0        0     2109 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_observation_py3.py
+-rw-rw-rw-   0        0        0     1255 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_py3.py
+-rw-rw-rw-   0        0        0     1447 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/related_report_response.py
+-rw-rw-rw-   0        0        0     1472 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/related_report_response_py3.py
+-rw-rw-rw-   0        0        0     1862 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator.py
+-rw-rw-rw-   0        0        0      741 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_class_permission.py
+-rw-rw-rw-   0        0        0      751 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1914 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_py3.py
+-rw-rw-rw-   0        0        0     1212 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_category_child.py
+-rw-rw-rw-   0        0        0     1257 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_category_child_py3.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_child.py
+-rw-rw-rw-   0        0        0     3005 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_child_py3.py
+-rw-rw-rw-   0        0        0     1828 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_create.py
+-rw-rw-rw-   0        0        0     1840 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_create_py3.py
+-rw-rw-rw-   0        0        0     1580 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_child.py
+-rw-rw-rw-   0        0        0     1626 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_child_py3.py
+-rw-rw-rw-   0        0        0     6134 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_create_request.py
+-rw-rw-rw-   0        0        0     6203 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_create_request_py3.py
+-rw-rw-rw-   0        0        0     3503 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_details_response.py
+-rw-rw-rw-   0        0        0     3557 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_details_response_py3.py
+-rw-rw-rw-   0        0        0     5911 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_edit_request.py
+-rw-rw-rw-   0        0        0     5970 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_edit_request_py3.py
+-rw-rw-rw-   0        0        0     2873 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_email_settings.py
+-rw-rw-rw-   0        0        0     2923 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_email_settings_py3.py
+-rw-rw-rw-   0        0        0     1384 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_details_response.py
+-rw-rw-rw-   0        0        0     1396 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_details_response_py3.py
+-rw-rw-rw-   0        0        0     3152 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_email_settings.py
+-rw-rw-rw-   0        0        0     3209 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_email_settings_py3.py
+-rw-rw-rw-   0        0        0     1089 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_report_settings.py
+-rw-rw-rw-   0        0        0     1099 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_report_settings_py3.py
+-rw-rw-rw-   0        0        0     2261 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_response.py
+-rw-rw-rw-   0        0        0     2298 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_response_py3.py
+-rw-rw-rw-   0        0        0     1820 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_edit.py
+-rw-rw-rw-   0        0        0     1832 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_edit_py3.py
+-rw-rw-rw-   0        0        0     1173 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_child_response.py
+-rw-rw-rw-   0        0        0     1209 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_child_response_py3.py
+-rw-rw-rw-   0        0        0     1134 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_request.py
+-rw-rw-rw-   0        0        0     1160 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_request_py3.py
+-rw-rw-rw-   0        0        0     1352 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_response.py
+-rw-rw-rw-   0        0        0     1382 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_response_py3.py
+-rw-rw-rw-   0        0        0     1841 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups.py
+-rw-rw-rw-   0        0        0      720 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_class_permission.py
+-rw-rw-rw-   0        0        0      730 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1893 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_py3.py
+-rw-rw-rw-   0        0        0     2949 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_child.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_child_py3.py
+-rw-rw-rw-   0        0        0     1519 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_day_indicator_child.py
+-rw-rw-rw-   0        0        0     1551 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_day_indicator_child_py3.py
+-rw-rw-rw-   0        0        0     3749 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_request.py
+-rw-rw-rw-   0        0        0     3794 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_request_py3.py
+-rw-rw-rw-   0        0        0     1350 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_child.py
+-rw-rw-rw-   0        0        0     1419 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_child_py3.py
+-rw-rw-rw-   0        0        0     1669 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_response.py
+-rw-rw-rw-   0        0        0     1739 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_response_py3.py
+-rw-rw-rw-   0        0        0     1189 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_type.py
+-rw-rw-rw-   0        0        0     1222 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_type_py3.py
+-rw-rw-rw-   0        0        0     1808 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports.py
+-rw-rw-rw-   0        0        0      687 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_class_permission.py
+-rw-rw-rw-   0        0        0      694 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1832 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_class_permission.py
+-rw-rw-rw-   0        0        0      719 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1882 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_py3.py
+-rw-rw-rw-   0        0        0     1857 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_py3.py
+-rw-rw-rw-   0        0        0     3920 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/required_address_child.py
+-rw-rw-rw-   0        0        0     3924 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/required_address_child_py3.py
+-rw-rw-rw-   0        0        0     1859 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords.py
+-rw-rw-rw-   0        0        0      738 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_class_permission.py
+-rw-rw-rw-   0        0        0      748 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1911 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_py3.py
+-rw-rw-rw-   0        0        0     1142 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reviewed.py
+-rw-rw-rw-   0        0        0     1152 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/reviewed_py3.py
+-rw-rw-rw-   0        0        0     1820 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles.py
+-rw-rw-rw-   0        0        0      699 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_class_permission.py
+-rw-rw-rw-   0        0        0      709 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1872 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_py3.py
+-rw-rw-rw-   0        0        0      992 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_detail.py
+-rw-rw-rw-   0        0        0      993 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_detail_py3.py
+-rw-rw-rw-   0        0        0     1471 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_response.py
+-rw-rw-rw-   0        0        0     1482 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_response_py3.py
+-rw-rw-rw-   0        0        0     1323 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update.py
+-rw-rw-rw-   0        0        0     1186 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_common_unit.py
+-rw-rw-rw-   0        0        0     1214 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_common_unit_py3.py
+-rw-rw-rw-   0        0        0     1348 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_py3.py
+-rw-rw-rw-   0        0        0     1059 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_child.py
+-rw-rw-rw-   0        0        0     1074 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_child_py3.py
+-rw-rw-rw-   0        0        0     1612 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_details_response.py
+-rw-rw-rw-   0        0        0     1628 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_details_response_py3.py
+-rw-rw-rw-   0        0        0     1133 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter.py
+-rw-rw-rw-   0        0        0     1452 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_channel_latest_reading_response.py
+-rw-rw-rw-   0        0        0     1460 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_channel_latest_reading_response_py3.py
+-rw-rw-rw-   0        0        0     1144 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_py3.py
+-rw-rw-rw-   0        0        0     2024 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_request.py
+-rw-rw-rw-   0        0        0     2025 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_request_py3.py
+-rw-rw-rw-   0        0        0     1312 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_response.py
+-rw-rw-rw-   0        0        0     1335 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_response_py3.py
+-rw-rw-rw-   0        0        0     1991 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments.py
+-rw-rw-rw-   0        0        0      870 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_class_permission.py
+-rw-rw-rw-   0        0        0      877 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2040 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_py3.py
+-rw-rw-rw-   0        0        0     5456 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_daily_data.py
+-rw-rw-rw-   0        0        0     5676 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_daily_data_py3.py
+-rw-rw-rw-   0        0        0     1826 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine.py
+-rw-rw-rw-   0        0        0      705 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_class_permission.py
+-rw-rw-rw-   0        0        0      712 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1875 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_py3.py
+-rw-rw-rw-   0        0        0     1757 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_log.py
+-rw-rw-rw-   0        0        0     1787 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_log_py3.py
+-rw-rw-rw-   0        0        0     3255 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_daily_response.py
+-rw-rw-rw-   0        0        0     3286 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_daily_response_py3.py
+-rw-rw-rw-   0        0        0     8969 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_response.py
+-rw-rw-rw-   0        0        0     9208 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_response_py3.py
+-rw-rw-rw-   0        0        0      779 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child.py
+-rw-rw-rw-   0        0        0      783 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_py3.py
+-rw-rw-rw-   0        0        0     3944 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_search_account_child.py
+-rw-rw-rw-   0        0        0     3993 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_search_account_child_py3.py
+-rw-rw-rw-   0        0        0     3885 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_meter_bill_entry.py
+-rw-rw-rw-   0        0        0     3949 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_meter_bill_entry_py3.py
+-rw-rw-rw-   0        0        0      790 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child.py
+-rw-rw-rw-   0        0        0      794 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_py3.py
+-rw-rw-rw-   0        0        0     2113 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_search_cost_center.py
+-rw-rw-rw-   0        0        0     2134 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_search_cost_center_py3.py
+-rw-rw-rw-   0        0        0      765 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child.py
+-rw-rw-rw-   0        0        0      769 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_py3.py
+-rw-rw-rw-   0        0        0     5794 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_search_meter_child.py
+-rw-rw-rw-   0        0        0     5842 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_search_meter_child_py3.py
+-rw-rw-rw-   0        0        0     1310 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_parent_place_child.py
+-rw-rw-rw-   0        0        0     1322 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_parent_place_child_py3.py
+-rw-rw-rw-   0        0        0      765 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child.py
+-rw-rw-rw-   0        0        0      769 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_py3.py
+-rw-rw-rw-   0        0        0     2374 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_search_place_child.py
+-rw-rw-rw-   0        0        0     2368 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_search_place_child_py3.py
+-rw-rw-rw-   0        0        0      731 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_group.py
+-rw-rw-rw-   0        0        0      735 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_group_py3.py
+-rw-rw-rw-   0        0        0     1762 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_response.py
+-rw-rw-rw-   0        0        0     1752 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_response_py3.py
+-rw-rw-rw-   0        0        0     2077 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_data_access_release_request.py
+-rw-rw-rw-   0        0        0     2068 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_data_access_release_request_py3.py
+-rw-rw-rw-   0        0        0     1856 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications.py
+-rw-rw-rw-   0        0        0      735 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_class_permission.py
+-rw-rw-rw-   0        0        0      745 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1908 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_py3.py
+-rw-rw-rw-   0        0        0     3655 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/setup.py
+-rw-rw-rw-   0        0        0     3634 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/setup_py3.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_request.py
+-rw-rw-rw-   0        0        0     2041 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_request_py3.py
+-rw-rw-rw-   0        0        0     1510 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_response.py
+-rw-rw-rw-   0        0        0     1538 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_response_py3.py
+-rw-rw-rw-   0        0        0     2114 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists.py
+-rw-rw-rw-   0        0        0      993 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_class_permission.py
+-rw-rw-rw-   0        0        0      997 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2160 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_py3.py
+-rw-rw-rw-   0        0        0     2135 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps.py
+-rw-rw-rw-   0        0        0     1014 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_class_permission.py
+-rw-rw-rw-   0        0        0     1018 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2181 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_py3.py
+-rw-rw-rw-   0        0        0     2108 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports.py
+-rw-rw-rw-   0        0        0      987 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_class_permission.py
+-rw-rw-rw-   0        0        0      991 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2154 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_py3.py
+-rw-rw-rw-   0        0        0      672 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_boolean.py
+-rw-rw-rw-   0        0        0      681 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_boolean_py3.py
+-rw-rw-rw-   0        0        0      670 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_value.py
+-rw-rw-rw-   0        0        0      673 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_value_py3.py
+-rw-rw-rw-   0        0        0     3821 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_create.py
+-rw-rw-rw-   0        0        0     3860 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_create_py3.py
+-rw-rw-rw-   0        0        0     3493 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_edit.py
+-rw-rw-rw-   0        0        0     3536 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_edit_py3.py
+-rw-rw-rw-   0        0        0     1704 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_method.py
+-rw-rw-rw-   0        0        0     1737 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_method_py3.py
+-rw-rw-rw-   0        0        0     3137 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_response.py
+-rw-rw-rw-   0        0        0     3186 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_response_py3.py
+-rw-rw-rw-   0        0        0     1452 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_type.py
+-rw-rw-rw-   0        0        0     1521 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_type_py3.py
+-rw-rw-rw-   0        0        0     3447 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_report_response.py
+-rw-rw-rw-   0        0        0     3488 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_report_response_py3.py
+-rw-rw-rw-   0        0        0     2394 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_widget_response.py
+-rw-rw-rw-   0        0        0     2412 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_widget_response_py3.py
+-rw-rw-rw-   0        0        0     2212 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request.py
+-rw-rw-rw-   0        0        0     2225 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2242 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response.py
+-rw-rw-rw-   0        0        0     2270 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response_py3.py
+-rw-rw-rw-   0        0        0     2073 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statistics_response.py
+-rw-rw-rw-   0        0        0     2090 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/statistics_response_py3.py
+-rw-rw-rw-   0        0        0     1068 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/submission_type_response.py
+-rw-rw-rw-   0        0        0     1101 2023-05-08 15:07:22.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/submission_type_response_py3.py
+-rw-rw-rw-   0        0        0     1394 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_request.py
+-rw-rw-rw-   0        0        0     1421 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_request_py3.py
+-rw-rw-rw-   0        0        0     1275 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_response.py
+-rw-rw-rw-   0        0        0     1296 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_response_py3.py
+-rw-rw-rw-   0        0        0     1317 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_request.py
+-rw-rw-rw-   0        0        0     1334 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_request_py3.py
+-rw-rw-rw-   0        0        0     1203 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_response.py
+-rw-rw-rw-   0        0        0     1214 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_response_py3.py
+-rw-rw-rw-   0        0        0     5610 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_request.py
+-rw-rw-rw-   0        0        0     5780 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_request_py3.py
+-rw-rw-rw-   0        0        0     3774 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_response.py
+-rw-rw-rw-   0        0        0     3914 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_response_py3.py
+-rw-rw-rw-   0        0        0      960 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_child.py
+-rw-rw-rw-   0        0        0      981 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_child_py3.py
+-rw-rw-rw-   0        0        0     2303 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_response.py
+-rw-rw-rw-   0        0        0     2352 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_response_py3.py
+-rw-rw-rw-   0        0        0     2088 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_with_hidden_request.py
+-rw-rw-rw-   0        0        0     2102 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_with_hidden_request_py3.py
+-rw-rw-rw-   0        0        0     1021 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_child.py
+-rw-rw-rw-   0        0        0     1033 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_child_py3.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_response.py
+-rw-rw-rw-   0        0        0     1042 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_response_py3.py
+-rw-rw-rw-   0        0        0      895 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/target.py
+-rw-rw-rw-   0        0        0      909 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_py3.py
+-rw-rw-rw-   0        0        0     1457 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_settings.py
+-rw-rw-rw-   0        0        0     1458 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_settings_py3.py
+-rw-rw-rw-   0        0        0      884 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_edit.py
+-rw-rw-rw-   0        0        0      891 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_edit_py3.py
+-rw-rw-rw-   0        0        0     3923 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_response.py
+-rw-rw-rw-   0        0        0     3933 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_response_py3.py
+-rw-rw-rw-   0        0        0     1145 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_type.py
+-rw-rw-rw-   0        0        0     1172 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_type_py3.py
+-rw-rw-rw-   0        0        0     1071 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_child.py
+-rw-rw-rw-   0        0        0     1095 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_child_py3.py
+-rw-rw-rw-   0        0        0     2991 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_line.py
+-rw-rw-rw-   0        0        0     3022 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_line_py3.py
+-rw-rw-rw-   0        0        0     2008 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_response.py
+-rw-rw-rw-   0        0        0     2012 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_response_py3.py
+-rw-rw-rw-   0        0        0     1635 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_vendor_line_request.py
+-rw-rw-rw-   0        0        0     1646 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_vendor_line_request_py3.py
+-rw-rw-rw-   0        0        0     1665 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_version.py
+-rw-rw-rw-   0        0        0     1674 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_version_py3.py
+-rw-rw-rw-   0        0        0      954 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_format_response.py
+-rw-rw-rw-   0        0        0      972 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_format_response_py3.py
+-rw-rw-rw-   0        0        0      967 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_data_response.py
+-rw-rw-rw-   0        0        0      966 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_data_response_py3.py
+-rw-rw-rw-   0        0        0     1146 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_entity.py
+-rw-rw-rw-   0        0        0     1155 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_entity_py3.py
+-rw-rw-rw-   0        0        0     1308 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_value.py
+-rw-rw-rw-   0        0        0     1315 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_value_py3.py
+-rw-rw-rw-   0        0        0     1086 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_child.py
+-rw-rw-rw-   0        0        0     1113 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_child_py3.py
+-rw-rw-rw-   0        0        0     1670 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_response.py
+-rw-rw-rw-   0        0        0     1719 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_response_py3.py
+-rw-rw-rw-   0        0        0      743 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/toggle_visible.py
+-rw-rw-rw-   0        0        0      754 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/toggle_visible_py3.py
+-rw-rw-rw-   0        0        0     2201 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request.py
+-rw-rw-rw-   0        0        0     2215 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2230 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response.py
+-rw-rw-rw-   0        0        0     2259 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1844 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_cost_center.py
+-rw-rw-rw-   0        0        0     1911 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_cost_center_py3.py
+-rw-rw-rw-   0        0        0     1825 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_place.py
+-rw-rw-rw-   0        0        0     1859 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_place_py3.py
+-rw-rw-rw-   0        0        0     2165 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request.py
+-rw-rw-rw-   0        0        0     2184 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request_py3.py
+-rw-rw-rw-   0        0        0     2290 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response.py
+-rw-rw-rw-   0        0        0     2324 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response_py3.py
+-rw-rw-rw-   0        0        0     1947 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_data_response.py
+-rw-rw-rw-   0        0        0     1947 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_data_response_py3.py
+-rw-rw-rw-   0        0        0     1737 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_target.py
+-rw-rw-rw-   0        0        0     1779 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_target_py3.py
+-rw-rw-rw-   0        0        0     3144 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_create.py
+-rw-rw-rw-   0        0        0     3144 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_create_py3.py
+-rw-rw-rw-   0        0        0     2519 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_edit.py
+-rw-rw-rw-   0        0        0     2525 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_edit_py3.py
+-rw-rw-rw-   0        0        0     1927 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_field_child.py
+-rw-rw-rw-   0        0        0     1934 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_field_child_py3.py
+-rw-rw-rw-   0        0        0     2733 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_response.py
+-rw-rw-rw-   0        0        0     2739 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_response_py3.py
+-rw-rw-rw-   0        0        0     1368 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_create.py
+-rw-rw-rw-   0        0        0     1371 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_create_py3.py
+-rw-rw-rw-   0        0        0     1738 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_edit.py
+-rw-rw-rw-   0        0        0     1752 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_edit_py3.py
+-rw-rw-rw-   0        0        0     1302 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_entity_response.py
+-rw-rw-rw-   0        0        0     1326 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_entity_response_py3.py
+-rw-rw-rw-   0        0        0     1233 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_response.py
+-rw-rw-rw-   0        0        0     1254 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_response_py3.py
+-rw-rw-rw-   0        0        0     1415 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_update.py
+-rw-rw-rw-   0        0        0     1429 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_update_py3.py
+-rw-rw-rw-   0        0        0     2406 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_update.py
+-rw-rw-rw-   0        0        0     2409 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_update_py3.py
+-rw-rw-rw-   0        0        0      948 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_value.py
+-rw-rw-rw-   0        0        0      954 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_value_py3.py
+-rw-rw-rw-   0        0        0     1468 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_child.py
+-rw-rw-rw-   0        0        0     1047 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_child_py3.py
+-rw-rw-rw-   0        0        0     1476 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_py3.py
+-rw-rw-rw-   0        0        0     1187 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_response.py
+-rw-rw-rw-   0        0        0     1195 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_response_py3.py
+-rw-rw-rw-   0        0        0     2411 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings.py
+-rw-rw-rw-   0        0        0     1290 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_class_permission.py
+-rw-rw-rw-   0        0        0     1292 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2455 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_py3.py
+-rw-rw-rw-   0        0        0     1071 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_type.py
+-rw-rw-rw-   0        0        0     1098 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_type_py3.py
+-rw-rw-rw-   0        0        0     1994 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills.py
+-rw-rw-rw-   0        0        0      873 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_class_permission.py
+-rw-rw-rw-   0        0        0      880 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2043 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_py3.py
+-rw-rw-rw-   0        0        0     1729 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_batch_status_request.py
+-rw-rw-rw-   0        0        0     1735 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_batch_status_request_py3.py
+-rw-rw-rw-   0        0        0      956 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_result.py
+-rw-rw-rw-   0        0        0      966 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_result_py3.py
+-rw-rw-rw-   0        0        0     1883 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills.py
+-rw-rw-rw-   0        0        0      762 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_class_permission.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1935 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_py3.py
+-rw-rw-rw-   0        0        0      753 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/updated_only_result.py
+-rw-rw-rw-   0        0        0      763 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/updated_only_result_py3.py
+-rw-rw-rw-   0        0        0     3283 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/upsert_aggregate_meter_request.py
+-rw-rw-rw-   0        0        0     3307 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/upsert_aggregate_meter_request_py3.py
+-rw-rw-rw-   0        0        0     1042 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child.py
+-rw-rw-rw-   0        0        0     1054 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_py3.py
+-rw-rw-rw-   0        0        0     1226 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_with_email.py
+-rw-rw-rw-   0        0        0     1235 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_with_email_py3.py
+-rw-rw-rw-   0        0        0     6659 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_create_request.py
+-rw-rw-rw-   0        0        0     6719 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_create_request_py3.py
+-rw-rw-rw-   0        0        0     8428 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_edit_request.py
+-rw-rw-rw-   0        0        0     8478 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_edit_request_py3.py
+-rw-rw-rw-   0        0        0      959 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_child.py
+-rw-rw-rw-   0        0        0      982 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_child_py3.py
+-rw-rw-rw-   0        0        0     2202 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_request.py
+-rw-rw-rw-   0        0        0     2213 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_request_py3.py
+-rw-rw-rw-   0        0        0     1642 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_response.py
+-rw-rw-rw-   0        0        0     1671 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_response_py3.py
+-rw-rw-rw-   0        0        0     1212 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_with_members.py
+-rw-rw-rw-   0        0        0     1229 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_with_members_py3.py
+-rw-rw-rw-   0        0        0     4386 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_response.py
+-rw-rw-rw-   0        0        0     4444 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_response_py3.py
+-rw-rw-rw-   0        0        0      816 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_role_request.py
+-rw-rw-rw-   0        0        0      831 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_role_request_py3.py
+-rw-rw-rw-   0        0        0     2301 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles.py
+-rw-rw-rw-   0        0        0      855 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_class_permission.py
+-rw-rw-rw-   0        0        0      862 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2350 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_py3.py
+-rw-rw-rw-   0        0        0     1991 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups.py
+-rw-rw-rw-   0        0        0      870 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_class_permission.py
+-rw-rw-rw-   0        0        0      877 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2040 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_py3.py
+-rw-rw-rw-   0        0        0      831 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform.py
+-rw-rw-rw-   0        0        0     3576 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_meter.py
+-rw-rw-rw-   0        0        0     3648 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_meter_py3.py
+-rw-rw-rw-   0        0        0      855 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_py3.py
+-rw-rw-rw-   0        0        0     1017 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_comparison.py
+-rw-rw-rw-   0        0        0     1029 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_comparison_py3.py
+-rw-rw-rw-   0        0        0      856 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_with_unit.py
+-rw-rw-rw-   0        0        0      857 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_with_unit_py3.py
+-rw-rw-rw-   0        0        0      922 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_audit_enable.py
+-rw-rw-rw-   0        0        0      939 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_audit_enable_py3.py
+-rw-rw-rw-   0        0        0     1083 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_child.py
+-rw-rw-rw-   0        0        0     1101 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_child_py3.py
+-rw-rw-rw-   0        0        0     2674 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_contract_response.py
+-rw-rw-rw-   0        0        0     2699 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_contract_response_py3.py
+-rw-rw-rw-   0        0        0     2372 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response.py
+-rw-rw-rw-   0        0        0     1966 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     1985 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     1810 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results.py
+-rw-rw-rw-   0        0        0     1857 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results_py3.py
+-rw-rw-rw-   0        0        0     2374 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1355 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_results.py
+-rw-rw-rw-   0        0        0     1384 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     2492 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_request.py
+-rw-rw-rw-   0        0        0     2502 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_request_py3.py
+-rw-rw-rw-   0        0        0     3119 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_response.py
+-rw-rw-rw-   0        0        0     3126 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_response_py3.py
+-rw-rw-rw-   0        0        0      976 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_type_child.py
+-rw-rw-rw-   0        0        0     1001 2023-05-08 15:07:20.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_type_child_py3.py
+-rw-rw-rw-   0        0        0     1320 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_udf_response.py
+-rw-rw-rw-   0        0        0     1329 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_udf_response_py3.py
+-rw-rw-rw-   0        0        0     2102 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors.py
+-rw-rw-rw-   0        0        0     1856 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module.py
+-rw-rw-rw-   0        0        0      735 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_class_permission.py
+-rw-rw-rw-   0        0        0      743 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_class_permission_py3.py
+-rw-rw-rw-   0        0        0     1906 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_py3.py
+-rw-rw-rw-   0        0        0      981 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_class_permission.py
+-rw-rw-rw-   0        0        0      987 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2150 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_py3.py
+-rw-rw-rw-   0        0        0     1034 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_child.py
+-rw-rw-rw-   0        0        0     1039 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_child_py3.py
+-rw-rw-rw-   0        0        0     1043 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_response.py
+-rw-rw-rw-   0        0        0     1048 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_response_py3.py
+-rw-rw-rw-   0        0        0      807 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point.py
+-rw-rw-rw-   0        0        0     1092 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_child.py
+-rw-rw-rw-   0        0        0     1131 2023-05-08 15:07:21.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_child_py3.py
+-rw-rw-rw-   0        0        0      831 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_py3.py
+-rw-rw-rw-   0        0        0      927 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_request.py
+-rw-rw-rw-   0        0        0      951 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_request_py3.py
+-rw-rw-rw-   0        0        0      756 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site.py
+-rw-rw-rw-   0        0        0      774 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_py3.py
+-rw-rw-rw-   0        0        0      876 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_request.py
+-rw-rw-rw-   0        0        0      894 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_request_py3.py
+-rw-rw-rw-   0        0        0     1404 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_result.py
+-rw-rw-rw-   0        0        0     1419 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_result_py3.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_settings.py
+-rw-rw-rw-   0        0        0     1349 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_settings_py3.py
+-rw-rw-rw-   0        0        0     1982 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings.py
+-rw-rw-rw-   0        0        0      861 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_class_permission.py
+-rw-rw-rw-   0        0        0      868 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_class_permission_py3.py
+-rw-rw-rw-   0        0        0     2031 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_py3.py
+-rw-rw-rw-   0        0        0     1658 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_child.py
+-rw-rw-rw-   0        0        0     1671 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_child_py3.py
+-rw-rw-rw-   0        0        0     1607 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_response.py
+-rw-rw-rw-   0        0        0     1631 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_response_py3.py
+-rw-rw-rw-   0        0        0     3584 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_summary.py
+-rw-rw-rw-   0        0        0     3712 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_summary_py3.py
+-rw-rw-rw-   0        0        0     2718 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_create_request.py
+-rw-rw-rw-   0        0        0     2724 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_create_request_py3.py
+-rw-rw-rw-   0        0        0     1292 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_custom_action.py
+-rw-rw-rw-   0        0        0     1290 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_custom_action_py3.py
+-rw-rw-rw-   0        0        0     3080 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_edit_request.py
+-rw-rw-rw-   0        0        0     3080 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_edit_request_py3.py
+-rw-rw-rw-   0        0        0     1105 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_event_type_child.py
+-rw-rw-rw-   0        0        0     1144 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_event_type_child_py3.py
+-rw-rw-rw-   0        0        0     1872 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_details_response.py
+-rw-rw-rw-   0        0        0     1866 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_details_response_py3.py
+-rw-rw-rw-   0        0        0     1475 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_response.py
+-rw-rw-rw-   0        0        0     1485 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_response_py3.py
+-rw-rw-rw-   0        0        0     3185 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_response.py
+-rw-rw-rw-   0        0        0     3209 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_response_py3.py
+-rw-rw-rw-   0        0        0     2900 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_create.py
+-rw-rw-rw-   0        0        0     2873 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_create_py3.py
+-rw-rw-rw-   0        0        0     2946 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_edit_py3.py
+-rw-rw-rw-   0        0        0     1453 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_response.py
+-rw-rw-rw-   0        0        0     1456 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_response_py3.py
+-rw-rw-rw-   0        0        0     3997 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response.py
+-rw-rw-rw-   0        0        0     2809 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_commodity_data.py
+-rw-rw-rw-   0        0        0     2895 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_commodity_data_py3.py
+-rw-rw-rw-   0        0        0     4083 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_py3.py
+-rw-rw-rw-   0        0        0     1995 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_results.py
+-rw-rw-rw-   0        0        0     2033 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_results_py3.py
+-rw-rw-rw-   0        0        0     1818 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_display_setting.py
+-rw-rw-rw-   0        0        0     1880 2023-05-08 15:07:23.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_display_setting_py3.py
+-rw-rw-rw-   0        0        0     2075 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_request.py
+-rw-rw-rw-   0        0        0     2050 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_request_py3.py
+-rw-rw-rw-   0        0        0     1874 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_response.py
+-rw-rw-rw-   0        0        0     1859 2023-05-08 15:07:25.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_response_py3.py
+-rw-rw-rw-   0        0        0      917 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/year_range.py
+-rw-rw-rw-   0        0        0      930 2023-05-08 15:07:24.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/models/year_range_py3.py
+-rw-rw-rw-   0        0        0      340 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/energycap/sdk/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:07:49.794090 EnergyCapSdk-8.2302.4532/setup.cfg
+-rw-rw-rw-   0        0        0      922 2023-05-08 15:07:19.000000 EnergyCapSdk-8.2302.4532/setup.py
```

### Comparing `EnergyCapSdk-8.2302.4520/EnergyCapSdk.egg-info/SOURCES.txt` & `EnergyCapSdk-8.2302.4532/EnergyCapSdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/energy_cap_api.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/energy_cap_api.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/__init__.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_cost_with_outlier_analysis_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_demand_with_outlier_analysis_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/abnormal_bill_use_with_outlier_analysis_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_alert_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_alert_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_audit_enable.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_audit_enable.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_audit_enable_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_audit_enable_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_with_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_with_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_child_with_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_child_with_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_code_history_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_code_history_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_connection_status_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_connection_status_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_connection_status_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_connection_status_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_digest_actual_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_digest_actual_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_with_serial_number.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_with_serial_number.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_child_with_serial_number_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_child_with_serial_number_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_rate_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_rate_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_rate_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_rate_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_meter_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_meter_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_or_meter_usage.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_or_meter_usage.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_or_meter_usage_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_or_meter_usage_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_period_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_period_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_rate_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_rate_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_template_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_template_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_template_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_template_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_udf_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_udf_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/account_udf_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/account_udf_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounting_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounting_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_actual_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_actual_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accounts_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accounts_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_processor_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_processor_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_processor_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_processor_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/accrual_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/accrual_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/actionable_bill_counts.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/actionable_bill_counts.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/actionable_bill_counts_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/actionable_bill_counts_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/activity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/activity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/activity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/activity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_lookup.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_lookup.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/address_lookup_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/address_lookup_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjusted_cost_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjusted_cost_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjusted_cost_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjusted_cost_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjustment_base_method_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjustment_base_method_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/adjustment_base_method_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/adjustment_base_method_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/admin_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/admin_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_comparison_response_ghg_performance_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_item_rank_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_item_rank_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_item_rank_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_item_rank_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_monthly_cap_trend_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_monthly_cap_trend_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_monthly_cap_trend_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_monthly_cap_trend_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_ghg_building_rank.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_ghg_building_rank.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_ghg_building_rank_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_ghg_building_rank_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_item_rank_with_unit_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_item_rank_with_unit_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/aggregated_response_item_rank_with_unit_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/aggregated_response_item_rank_with_unit_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/all_installed_reports_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/all_installed_reports_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_create_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_create_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_edit_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_edit_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_edit_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_edit_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_key_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_key_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_user.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_user.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/api_user_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/api_user_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/application_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/application_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_request_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_request_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_request_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_request_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approval_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approval_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/approve_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/approve_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/assign_versions_to_step.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/assign_versions_to_step.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/assign_versions_to_step_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/assign_versions_to_step_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/auc_range_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/auc_range_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/audit_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/audit_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_engine_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_engine_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_log.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_log.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_log_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_log_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_baseline_bill.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_baseline_bill.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_baseline_bill_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_baseline_bill_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_baseline_bill.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_baseline_bill.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_baseline_bill_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_baseline_bill_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/baseline_processor_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/baseline_processor_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/batch_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/batch_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_category_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_category_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_category_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_category_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_value_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_value_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_values_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_values_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_values_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_values_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_with_used_count_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_with_used_count_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/benchmark_with_used_count_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/benchmark_with_used_count_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_body_line_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_body_line_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_statistics_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_account_meter_statistics_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_account_meter_statistics_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_accrual_exclusion_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_accrual_exclusion_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_accrual_exclusion_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_accrual_exclusion_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_approve.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_approve.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_approve_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_approve_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_custom.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_custom.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_custom_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_custom_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_delete.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_delete.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_delete_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_delete_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_export_hold.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_export_hold.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_export_hold_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_export_hold_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_header_update.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_header_update.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_header_update_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_header_update_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_historical_export.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_historical_export.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_historical_export_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_historical_export_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_list.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_list.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_list_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_list_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_move_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_move_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_split.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_split.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_split_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_split_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_void.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_void.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_action_void_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_action_void_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_calendarized_history.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_calendarized_history.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_calendarized_history_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_calendarized_history_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_descriptions_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_contains_line_item_types_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_contains_line_item_types_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_delete_action_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_delete_action_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_delete_action_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_delete_action_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_with_noun_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_with_noun_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_body_line_with_noun_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_body_line_with_noun_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_observation_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_observation_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_observation_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_observation_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_entry_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_entry_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_options.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_options.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_options_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_options_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_export_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_export_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_account_period_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_account_period_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_account_period_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_account_period_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_begin_date_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_begin_date_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_begin_date_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_begin_date_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_billing_period_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_billing_period_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_billing_period_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_billing_period_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_control_code_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_control_code_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_control_code_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_control_code_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_due_date_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_due_date_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_due_date_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_due_date_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_end_date_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_end_date_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_end_date_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_end_date_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_estimated_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_estimated_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_estimated_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_estimated_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_invoice_number_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_invoice_number_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_invoice_number_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_invoice_number_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_statement_date_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_statement_date_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_update_statement_date_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_update_statement_date_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_workflow_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_workflow_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_header_workflow_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_header_workflow_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_history_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_history_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_history_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_history_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_id_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_id_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_id_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_id_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_column_mapping.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_column_mapping.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_column_mapping_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_column_mapping_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_observation.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_observation.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_observation_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_observation_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_profile_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_profile_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_import_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_import_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_list_administrator_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_list_administrator_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_body_line_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_body_line_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_meter_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_meter_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_file_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_file_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_file_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_file_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_item.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_item.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_item_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_item_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_payment_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_payment_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_reversal_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_reversal_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_significantly_shorter_or_longer_than_previous_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_parent_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_parent_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_parent_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_parent_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_place_size_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_place_size_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_split_place_size_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_split_place_size_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_options.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_options.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_options_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_options_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_unexport_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_unexport_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_usage.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_usage.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_usage_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_usage_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_address_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_address_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_address_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_address_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_vendor_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_vendor_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_view_vendor_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_view_vendor_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bill_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bill_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_delta_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_delta_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_cost_unit_delta_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_cost_unit_delta_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_delta_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_delta_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_cost_delta_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_cost_delta_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_delta_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_delta_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/billing_period_use_unit_delta_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/billing_period_use_unit_delta_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_and_batches_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_and_batches_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_overdue_from_vendor_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_overdue_from_vendor_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bills_overdue_from_vendor_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bills_overdue_from_vendor_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bodyline_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bodyline_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/budgets_and_budget_versions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/budgets_and_budget_versions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/building_and_meter_groups_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/building_and_meter_groups_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_actual_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_actual_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_calendarized_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_calendarized_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_meter_interval_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_normalized_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_normalized_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_savings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_savings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_meters_module_sustainability_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_meters_module_sustainability_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/buildings_and_organizations_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/buildings_and_organizations_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_baseline_processor_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_baseline_processor_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_baseline_processor_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_baseline_processor_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_meter_cost_avoidance_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_meter_cost_avoidance_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/bulk_meter_cost_avoidance_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/bulk_meter_cost_avoidance_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculate_savings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculate_savings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculate_savings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculate_savings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_cost_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_cost_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_demand_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_demand_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculated_bill_use_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculated_bill_use_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calculation_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calculation_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_calculation_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_calculation_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_sum_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_sum_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/calendarized_sum_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/calendarized_sum_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_with_observation_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_with_observation_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_child_with_observation_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_child_with_observation_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_latest_reading.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_latest_reading.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_latest_reading_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_latest_reading_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_with_begin_date_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_with_begin_date_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/channel_version_with_begin_date_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/channel_version_with_begin_date_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_aggregations.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_aggregations.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_aggregations_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_aggregations_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_splits.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_splits.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_for_splits_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_for_splits_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_without_filters.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_without_filters.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_processor_settings_without_filters_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_processor_settings_without_filters_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_reversals_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_reversals_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_version_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_version_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_task_version_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_task_version_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_base.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_base.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_base_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_base_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_split_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_split_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_digest_split_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_digest_split_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargeback_workflow_step_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargeback_workflow_step_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/chargebacks_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/chargebacks_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/claim.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/claim.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/claim_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/claim_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_digest_actual_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_digest_actual_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_value_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_value_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/commodity_value_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/commodity_value_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/contact_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/contact_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/contact_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/contact_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_from_meter_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_from_meter_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_from_meter_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_from_meter_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_meter_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_meter_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/copy_meter_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/copy_meter_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_task.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_task.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_avoidance_task_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_avoidance_task_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_digest_actual_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_digest_actual_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_center_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_center_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_centers_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_centers_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_unit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_unit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/cost_savings_unit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/cost_savings_unit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/country.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/country.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/country_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/country_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_template_from_bill.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_template_from_bill.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_template_from_bill_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_template_from_bill_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_utility_platform_meter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_utility_platform_meter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/create_utility_platform_meter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/create_utility_platform_meter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/customer_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/customer_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_administrator_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_administrator_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_and_maps_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_and_maps_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_copy.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_copy.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_copy_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_copy_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_global_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_global_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dashboard_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dashboard_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_meta_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_meta_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_meta_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_meta_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_no_file_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_no_file_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_no_file_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_no_file_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_state.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_state.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_state_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_state_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_status.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_status.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_access_release_status_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_access_release_status_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/data_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/data_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/delete_reading_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/delete_reading_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/delete_reading_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/delete_reading_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/destination_account_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/destination_account_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_base.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_base.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_base_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_base_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_to_bills_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_to_bills_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribute_account_charges_to_bills_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribute_account_charges_to_bills_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_configuration.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_configuration.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_configuration_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_configuration_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distributed_reports_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distributed_reports_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_manage.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_manage.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_manage_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_manage_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/distribution_version_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/distribution_version_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/due_date_too_long_after_bill_end_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_list_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_list_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_list_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_list_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/dynamic_percentage_bill_split_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/dynamic_percentage_bill_split_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/email_properties.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/email_properties.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/email_properties_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/email_properties_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_cap_options_energy_cap_id_options.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_cap_options_energy_cap_id_options.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_cap_options_energy_cap_id_options_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_cap_options_energy_cap_id_options_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_project_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_project_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_unit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_unit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_savings_unit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_savings_unit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_commodity_meter_type_mapping_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_commodity_meter_type_mapping_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_meter_link_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_meter_link_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_hierarchy_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_hierarchy_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_hierarchy_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_link_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_link_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_metrics_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_metrics_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_place_submission_status_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_place_submission_status_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_meter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_meter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_meter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_meter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_property.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_property.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_pm_property_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_pm_property_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_rating_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_rating_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_rating_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_rating_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_submission_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_submission_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energy_star_task_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energy_star_task_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/energystar_submissions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/energystar_submissions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/environment.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/environment.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/environment_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/environment_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/estimated.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/estimated.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/estimated_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/estimated_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_format_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_format_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_format_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_format_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_hold_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_hold_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/export_workflow_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/export_workflow_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/facility_projects_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/facility_projects_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_reading_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_reading_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_reading_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_reading_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_readings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_readings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/failed_readings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/failed_readings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/file_data_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/file_data_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/file_data_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/file_data_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_data_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_data_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_data_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_data_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/filter_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/filter_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_amount_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_amount_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_amount_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_amount_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_demand_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_demand_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_demand_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_demand_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_percentage_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_percentage_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_unit_cost_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_unit_cost_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_unit_cost_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_unit_cost_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_use_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_use_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/fixed_use_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/fixed_use_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_action_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_action_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_action_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_action_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_event_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_event_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_event_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_event_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_issue_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_issue_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_issue_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_issue_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_list_action.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_list_action.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_list_action_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_list_action_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_status_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_status_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_status_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_status_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_type_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_type_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flag_widget_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flag_widget_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/flagged_items_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/flagged_items_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/floor_area_split_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/floor_area_split_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/form_template_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/form_template_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/frequency.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/frequency.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/frequency_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/frequency_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/general_ledger_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/general_ledger_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_bodyline_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_bodyline_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_count.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_count.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/generic_count_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/generic_count_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_building_rank.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_building_rank.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_building_rank_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_building_rank_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_carbon_footprint_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_carbon_footprint_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_carbon_footprint_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_carbon_footprint_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_factor.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_factor.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_factor_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_factor_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_default_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_default_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_by_category_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_by_category_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_by_category_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_by_category_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_category_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_category_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_version_history_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_version_history_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factor_version_history_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factor_version_history_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factors_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factors_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_factors_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_factors_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_gas.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_gas.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_gas_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_gas_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_group_emissions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_group_emissions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_group_emissions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_group_emissions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_performance_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_performance_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_performance_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_performance_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_category_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_category_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_scope_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_scope_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_target_emissions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_target_emissions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_target_emissions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_target_emissions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_version.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_version.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_version_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_version_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_yearly_emissions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_yearly_emissions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ghg_yearly_emissions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ghg_yearly_emissions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_sub_code_child_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_sub_code_child_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/gl_subcode_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/gl_subcode_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/global_cost_avoidance_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/global_cost_avoidance_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/greenhouse_gas_administrator_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/greenhouse_gas_administrator_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_display_setting.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_display_setting.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_display_setting_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_display_setting_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_member_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_member_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_member_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_meter_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_meter_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_meter_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_meter_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_member.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_member.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_member_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_member_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/group_place_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/group_place_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/groups_and_benchmarks_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/groups_and_benchmarks_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/guid_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/guid_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/guid_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/guid_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hidden_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hidden_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hidden_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hidden_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers2.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers2.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers2_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers2_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_cost_centers_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_cost_centers_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places2.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places2.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places2_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places2_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/hierarchical_places_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/hierarchical_places_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_analysis_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_analysis_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/interval_data_rollup_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/interval_data_rollup_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_with_unit_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_with_unit_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/item_rank_with_unit_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/item_rank_with_unit_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/latest_benchmark_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/latest_benchmark_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/latest_benchmark_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/latest_benchmark_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accounting_export.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accounting_export.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accounting_export_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accounting_export_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accrual_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accrual_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_accrual_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_accrual_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_chargebacks.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_chargebacks.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_chargebacks_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_chargebacks_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_cost_avoidance.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_cost_avoidance.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_cost_avoidance_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_cost_avoidance_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_custom_benchmarks.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_custom_benchmarks.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_custom_benchmarks_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_custom_benchmarks_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_ghg.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_ghg.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_ghg_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_ghg_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_interval_data_analysis.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_interval_data_analysis.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_interval_data_analysis_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_interval_data_analysis_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_designer.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_designer.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_designer_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_designer_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_distribution.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_distribution.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_feature_report_distribution_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_feature_report_distribution_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_features.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_features.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_features_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_features_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/license_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/license_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_accrual_exclusion.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_accrual_exclusion.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_accrual_exclusion_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_accrual_exclusion_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_approve.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_approve.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_approve_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_approve_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_custom.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_custom.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_custom_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_custom_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_export_hold.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_export_hold.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_export_hold_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_export_hold_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_reverse.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_reverse.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_reverse_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_reverse_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_void.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_void.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_action_void_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_action_void_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_column_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_column_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_column_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_column_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_copy.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_copy.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_copy_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_copy_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_create_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_create_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_ids.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_ids.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_ids_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_ids_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_field.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_field.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_field_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_field_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_item.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_item.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_list_item_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_list_item_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/list_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/list_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/login_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/login_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manual_adjustment_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manual_adjustment_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manual_adjustment_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manual_adjustment_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/manually_adjust_savings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/manually_adjust_savings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_dashboard_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_dashboard_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_widget_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_widget_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/map_widget_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/map_widget_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/me.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/me.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/me_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/me_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/message.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/message_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/message_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_bill_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_bill_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_bill_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_bill_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_calendarized_use_vs_weather_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_calendarized_use_vs_weather_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_calendarized_use_vs_weather_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_calendarized_use_vs_weather_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cap_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cap_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cap_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cap_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_category_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_category_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_meter_import_id_and_route.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_meter_import_id_and_route.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_meter_import_id_and_route_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_meter_import_id_and_route_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_and_serial_number.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_and_serial_number.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_and_serial_number_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_and_serial_number_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_channel_latest_reading.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_channel_latest_reading.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_include_place_channel_latest_reading_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_include_place_channel_latest_reading_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_search.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_search.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_child_search_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_child_search_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cost.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cost.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_cost_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_cost_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_actual_and_calendarized_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_calendarized_trend_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_calendarized_trend_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_scope_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_ghg_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_ghg_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_ghg_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_normalized_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_normalized_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_digest_savings_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_digest_savings_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_category_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_category_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_category_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_category_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_demand_ranking_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_demand_ranking_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_digest_ranking_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_digest_ranking_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_member_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_member_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_rate_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_rate_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_rate_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_rate_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_savings_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_savings_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_search_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_search_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_search_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_search_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_serial_number_history_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_serial_number_history_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_template_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_template_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_template_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_template_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_udf_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_udf_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meter_udf_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meter_udf_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/meters_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/meters_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/missing_bill_widget.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/missing_bill_widget.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/missing_bill_widget_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/missing_bill_widget_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/monthly_cap_trend.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/monthly_cap_trend.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/monthly_cap_trend_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/monthly_cap_trend_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/most_recent_aggregate.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/most_recent_aggregate.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/most_recent_aggregate_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/most_recent_aggregate_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_accounts_between_vendors_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_accounts_between_vendors_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_bills_destination.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_bills_destination.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_bills_destination_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_bills_destination_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_create_meter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_create_meter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_create_meter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_create_meter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/move_existing_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/move_existing_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/named_period.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/named_period.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/named_period_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/named_period_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/normalization_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/normalization_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_action_button_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_action_button_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_action_button_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_action_button_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_badge_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_badge_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_badge_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_badge_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_category.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_category.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_category_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_category_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_system_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_system_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_system_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_system_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_update_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_update_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/notification_update_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/notification_update_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_method_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_method_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_method_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_method_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_rule.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_rule.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_rule_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_rule_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_base.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_base.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_base_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_base_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/observation_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/observation_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_object_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_object_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_object_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_object_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/ok_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/ok_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_category_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_category_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/other_savings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/other_savings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/outlier_severity_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/outlier_severity_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/outlier_severity_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/outlier_severity_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_detailed.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_detailed.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_detailed_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_detailed_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_range_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_range_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/period_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/period_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/permissions_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/permissions_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_category_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_category_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_with_floor_area.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_with_floor_area.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_child_with_floor_area_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_child_with_floor_area_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_cost.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_cost.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_cost_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_cost_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_actual_and_calendarized_yearly_response_target_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_comparison_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_comparison_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_comparison_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_comparison_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_commodity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_eui_energy_project_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_energy_use_intensity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_energy_use_intensity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_commodity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_scope_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_ghg_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_monthly_response_target_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_scope_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_ghg_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_ghg_yearly_response_target_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_commodity_target_comparison_monthly_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_target_comparison_monthly_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_normalized_yearly_response_target_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_monthly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_monthly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_savings_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_savings_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_digest_target_comparison_monthly_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_digest_target_comparison_monthly_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_category_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_category_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_category_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_category_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_area_ranking_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_area_ranking_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_benchmark_ranking_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_benchmark_ranking_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_digest_weather_ranking_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_digest_weather_ranking_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_member.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_member.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_member_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_member_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_info.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_info.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_info_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_info_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_size_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_size_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_submission_type_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_submission_type_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_submission_type_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_submission_type_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_udf_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_udf_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/place_udf_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/place_udf_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/pm_commodity_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/pm_commodity_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/pm_commodity_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/pm_commodity_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_weather_station.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_weather_station.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/postal_code_response_weather_station_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/postal_code_response_weather_station_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/preference_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/preference_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/primary_use_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/primary_use_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/project_manager_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/project_manager_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/project_manager_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/project_manager_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/public_dashboards_or_maps_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/public_dashboards_or_maps_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_filter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_filter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_filter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_filter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_report.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_report.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/quick_report_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/quick_report_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_child_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_child_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_digest_actual_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_digest_actual_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_schedules_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_schedules_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rate_version_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rate_version_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_child_base.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_child_base.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_child_base_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_child_base_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_delete.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_delete.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_delete_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_delete_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_column.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_column.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_column_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_column_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_profile_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_profile_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_import_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_import_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reading_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reading_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_observation.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_observation.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_observation_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_observation_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/readings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/readings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/related_report_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/related_report_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/related_report_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/related_report_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_administrator_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_administrator_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_category_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_category_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_category_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_category_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_create_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_create_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_create_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_create_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_edit_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_edit_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_edit_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_edit_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_email_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_email_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_email_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_email_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_email_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_email_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_email_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_email_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_report_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_report_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_report_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_report_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_distribution_log_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_distribution_log_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_child_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_child_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_child_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_child_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_groups_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_groups_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_day_indicator_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_day_indicator_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_day_indicator_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_day_indicator_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_subscription_schedule_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_subscription_schedule_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/report_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/report_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reports_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reports_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/required_address_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/required_address_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/required_address_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/required_address_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reset_user_passwords_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reset_user_passwords_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reviewed.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reviewed.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/reviewed_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/reviewed_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/roles_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/roles_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_detail.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_detail.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_detail_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_detail_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rolling_comparison_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rolling_comparison_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_common_unit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_common_unit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_common_unit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_common_unit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/rollup_unit_update_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/rollup_unit_update_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_channel_latest_reading_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_channel_latest_reading_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_channel_latest_reading_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_channel_latest_reading_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_meter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_meter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/route_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/route_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_adjustments_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_adjustments_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_daily_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_daily_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_daily_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_daily_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_engine_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_engine_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_log.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_log.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_log_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_log_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_daily_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_daily_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_daily_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_daily_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/savings_meter_bill_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/savings_meter_bill_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_search_account_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_search_account_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_child_search_account_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_child_search_account_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_meter_bill_entry.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_meter_bill_entry.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_account_meter_bill_entry_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_account_meter_bill_entry_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_search_cost_center.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_search_cost_center.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_cost_center_child_search_cost_center_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_cost_center_child_search_cost_center_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_search_meter_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_search_meter_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_meter_child_search_meter_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_meter_child_search_meter_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_parent_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_parent_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_parent_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_parent_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_search_place_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_search_place_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_child_search_place_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_child_search_place_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_group.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_group.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_place_group_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_place_group_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/search_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/search_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_data_access_release_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_data_access_release_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_data_access_release_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_data_access_release_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/send_notifications_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/send_notifications_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/setup.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/setup.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/setup_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/setup_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/share_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/share_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_bill_lists_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_bill_lists_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_dashboards_or_maps_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_dashboards_or_maps_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/shared_reports_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/shared_reports_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_boolean.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_boolean.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_boolean_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_boolean_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/single_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/single_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_method.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_method.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_method_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_method_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/special_adjustment_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/special_adjustment_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_report_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_report_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_report_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_report_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_widget_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_widget_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/specific_widget_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/specific_widget_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statement_date_too_long_after_bill_end_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statistics_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statistics_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/statistics_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/statistics_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/submission_type_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/submission_type_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/submission_type_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/submission_type_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/subtract_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/subtract_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/sum_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/sum_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_with_hidden_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_with_hidden_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/system_user_role_with_hidden_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/system_user_role_with_hidden_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/tag_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/tag_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/target.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/target.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/target_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/target_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/task_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/task_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_line.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_line.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_line_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_line_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_vendor_line_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_vendor_line_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_vendor_line_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_vendor_line_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_version.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_version.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/template_version_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/template_version_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_format_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_format_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_format_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_format_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_data_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_data_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_data_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_data_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_entity.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_entity.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_entity_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_entity_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_series_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_series_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/time_zone_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/time_zone_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/toggle_visible.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/toggle_visible.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/toggle_visible_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/toggle_visible_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/too_many_consecutive_estimated_bills_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_cost_center.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_cost_center.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_cost_center_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_cost_center_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_place.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_place.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/topmost_place_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/topmost_place_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/total_bill_cost_does_not_match_line_item_types_setting_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_data_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_data_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_data_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_data_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_target.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_target.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/trend_target_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/trend_target_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_field_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_field_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_field_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_field_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_entity_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_entity_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_entity_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_entity_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_update.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_update.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_select_value_update_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_select_value_update_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_update.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_update.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_update_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_update_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_value.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_value.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/udf_value_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/udf_value_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_system_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_system_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_type.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_type.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/unit_type_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/unit_type_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_approved_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_approved_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_batch_status_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_batch_status_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_batch_status_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_batch_status_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/update_units_on_existing_bills_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/update_units_on_existing_bills_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/updated_only_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/updated_only_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/updated_only_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/updated_only_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/upsert_aggregate_meter_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/upsert_aggregate_meter_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/upsert_aggregate_meter_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/upsert_aggregate_meter_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_with_email.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_with_email.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_child_with_email_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_child_with_email_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_create_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_create_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_create_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_create_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_edit_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_edit_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_edit_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_edit_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_with_members.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_with_members.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_group_with_members_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_group_with_members_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_role_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_role_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/user_role_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/user_role_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_roles_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_roles_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/users_and_user_groups_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/users_and_user_groups_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_meter.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_meter.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_meter_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_meter_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/utility_platform_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/utility_platform_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_comparison.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_comparison.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_comparison_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_comparison_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_with_unit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_with_unit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/value_with_unit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/value_with_unit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_audit_enable.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_audit_enable.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_audit_enable_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_audit_enable_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_contract_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_contract_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_contract_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_contract_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_commodity_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_digest_actual_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_digest_actual_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_udf_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_udf_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendor_udf_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendor_udf_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_and_rates_module_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_and_rates_module_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/vendors_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/vendors_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/version_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/version_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_data_point_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_data_point_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/wattics_site_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/wattics_site_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_result.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_result.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_result_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_result_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_import_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_import_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_class_permission.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_class_permission.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_class_permission_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_class_permission_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_settings_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_settings_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_summary.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_summary.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/weather_station_summary_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/weather_station_summary_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_create_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_create_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_create_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_create_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_custom_action.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_custom_action.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_custom_action_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_custom_action_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_edit_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_edit_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_edit_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_edit_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_event_type_child.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_event_type_child.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_event_type_child_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_event_type_child_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_details_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_details_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_details_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_details_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_log_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_log_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/webhook_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/webhook_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_create.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_create.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_create_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_create_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_edit.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_edit.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_edit_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_edit_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_commodity_data.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_commodity_data.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_commodity_data_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_commodity_data_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_results.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_results.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/widget_savings_yearly_response_results_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/widget_savings_yearly_response_results_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_display_setting.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_display_setting.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_display_setting_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_display_setting_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_request.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_request.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_request_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_request_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_response.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_response.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/workflow_settings_response_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/workflow_settings_response_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/year_range.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/year_range.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/energycap/sdk/models/year_range_py3.py` & `EnergyCapSdk-8.2302.4532/energycap/sdk/models/year_range_py3.py`

 * *Files identical despite different names*

### Comparing `EnergyCapSdk-8.2302.4520/setup.py` & `EnergyCapSdk-8.2302.4532/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "EnergyCapSdk"
-VERSION = "8.2302.4520"
+VERSION = "8.2302.4532"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```


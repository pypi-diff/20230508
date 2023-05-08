# Comparing `tmp/dt-1.1.59.tar.gz` & `tmp/dt-1.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-1.1.59.tar", last modified: Tue Apr 18 19:21:02 2023, max compression
+gzip compressed data, was "dt-1.1.60.tar", last modified: Mon May  8 21:12:03 2023, max compression
```

## Comparing `dt-1.1.59.tar` & `dt-1.1.60.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.598117 dt-1.1.59/
--rw-r--r--   0 runner    (1001) docker     (122)    10765 2023-04-18 19:20:55.000000 dt-1.1.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-04-18 19:21:02.598117 dt-1.1.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14717 2023-04-18 19:20:55.000000 dt-1.1.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.590117 dt-1.1.59/dt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-04-18 19:21:02.000000 dt-1.1.59/dt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-18 19:21:02.000000 dt-1.1.59/dt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 19:21:02.000000 dt-1.1.59/dt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-18 19:21:02.000000 dt-1.1.59/dt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-18 19:21:02.000000 dt-1.1.59/dt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.590117 dt-1.1.59/dynatrace/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.590117 dt-1.1.59/dynatrace/configuration_v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15903 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/alerting_profiles.py
--rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/anomaly_detection_process_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    18522 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/auto_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/credential_vault.py
--rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (122)    11959 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/geographic_regions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11449 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (122)     5557 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/management_zones.py
--rw-r--r--   0 runner    (1001) docker     (122)    10974 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/metric_events.py
--rw-r--r--   0 runner    (1001) docker     (122)    13214 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/notifications.py
--rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/oneagent_environment_wide_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/oneagent_in_a_hostgroup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8512 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/oneagent_on_a_host.py
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/configuration_v1/tile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/dynatrace_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.594117 dt-1.1.59/dynatrace/environment_v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/cluster_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     8039 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/custom_device.py
--rw-r--r--   0 runner    (1001) docker     (122)    19922 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     4653 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     6647 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/oneagents.py
--rw-r--r--   0 runner    (1001) docker     (122)     5320 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/smartscape_hosts.py
--rw-r--r--   0 runner    (1001) docker     (122)     6103 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/synthetic_monitors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/synthetic_third_party.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v1/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.594117 dt-1.1.59/dynatrace/environment_v2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/activegates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/activegates_autoupdate_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     5487 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/activegates_autoupdate_jobs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)    10148 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/events.py
--rw-r--r--   0 runner    (1001) docker     (122)    13717 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     8967 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    15456 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/monitored_entities.py
--rw-r--r--   0 runner    (1001) docker     (122)     4193 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/networkzones.py
--rw-r--r--   0 runner    (1001) docker     (122)    14388 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/problems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    12254 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/service_level_objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     8928 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1848 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/environment_v2/tokens_tenant.py
--rw-r--r--   0 runner    (1001) docker     (122)     5361 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7902 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/pagination.py
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-04-18 19:20:55.000000 dt-1.1.59/dynatrace/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 19:21:02.598117 dt-1.1.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-04-18 19:20:55.000000 dt-1.1.59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.594117 dt-1.1.59/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.598117 dt-1.1.59/test/configuration_v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_alerting_profiles.py
--rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_anomaly_detection_metric_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_auto_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_management_zones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_oneagent_environment_wide_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_oneagent_in_a_hostgroup.py
--rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-04-18 19:20:55.000000 dt-1.1.59/test/configuration_v1/test_oneagent_on_a_host.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-18 19:20:55.000000 dt-1.1.59/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.598117 dt-1.1.59/test/environment_v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v1/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v1/test_smartscape_hosts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v1/test_synthetic_monitors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:21:02.598117 dt-1.1.59/test/environment_v2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_activegate_autoupdate_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_activegate_autoupdate_jobs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_customtags.py
--rw-r--r--   0 runner    (1001) docker     (122)     7167 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3604 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_events_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_networkzones.py
--rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_problems.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_service_level_objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-18 19:20:55.000000 dt-1.1.59/test/environment_v2/test_tokens_tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.218338 dt-1.1.60/
+-rw-r--r--   0 runner    (1001) docker     (122)    10765 2023-05-08 21:12:00.000000 dt-1.1.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-08 21:12:03.218338 dt-1.1.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14717 2023-05-08 21:12:00.000000 dt-1.1.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.206339 dt-1.1.60/dt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-08 21:12:03.000000 dt-1.1.60/dt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-05-08 21:12:03.000000 dt-1.1.60/dt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 21:12:03.000000 dt-1.1.60/dt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-08 21:12:03.000000 dt-1.1.60/dt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-08 21:12:03.000000 dt-1.1.60/dt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.206339 dt-1.1.60/dynatrace/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.210338 dt-1.1.60/dynatrace/configuration_v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15903 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/alerting_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/anomaly_detection_process_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18522 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/auto_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/credential_vault.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11959 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/geographic_regions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11449 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5557 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/management_zones.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10974 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/metric_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13214 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/oneagent_environment_wide_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/oneagent_in_a_hostgroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8512 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/oneagent_on_a_host.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/configuration_v1/tile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/dynatrace_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.210338 dt-1.1.60/dynatrace/environment_v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/cluster_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8039 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/custom_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19922 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4653 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6647 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/oneagents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5320 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/smartscape_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6103 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/synthetic_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/synthetic_third_party.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v1/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.214338 dt-1.1.60/dynatrace/environment_v2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/activegates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/activegates_autoupdate_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5487 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/activegates_autoupdate_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10148 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13717 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8967 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15456 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/monitored_entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4193 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/networkzones.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14388 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/problems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12254 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/service_level_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8928 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1848 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/environment_v2/tokens_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5361 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7902 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-08 21:12:00.000000 dt-1.1.60/dynatrace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 21:12:03.218338 dt-1.1.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-05-08 21:12:00.000000 dt-1.1.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.214338 dt-1.1.60/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.214338 dt-1.1.60/test/configuration_v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_alerting_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_anomaly_detection_metric_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_auto_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_management_zones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_oneagent_environment_wide_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_oneagent_in_a_hostgroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-05-08 21:12:00.000000 dt-1.1.60/test/configuration_v1/test_oneagent_on_a_host.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-08 21:12:00.000000 dt-1.1.60/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.214338 dt-1.1.60/test/environment_v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v1/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v1/test_smartscape_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v1/test_synthetic_monitors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:03.218338 dt-1.1.60/test/environment_v2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_activegate_autoupdate_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_activegate_autoupdate_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_customtags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7167 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3604 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_events_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_networkzones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_problems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_service_level_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-08 21:12:00.000000 dt-1.1.60/test/environment_v2/test_tokens_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-08 21:12:00.000000 dt-1.1.60/test/test_logs.py
```

### Comparing `dt-1.1.59/LICENSE` & `dt-1.1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/PKG-INFO` & `dt-1.1.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dt
-Version: 1.1.59
+Version: 1.1.60
 Summary: Dynatrace API Python client
 Home-page: https://github.com/dlopes7/dynatrace-rest-python
 Author: David Lopes
 Author-email: davidribeirolopes@gmail.com
 Project-URL: Issue Tracker, https://github.com/dlopes7/dynatrace-rest-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dt-1.1.59/README.md` & `dt-1.1.60/README.md`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dt.egg-info/PKG-INFO` & `dt-1.1.60/dt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dt
-Version: 1.1.59
+Version: 1.1.60
 Summary: Dynatrace API Python client
 Home-page: https://github.com/dlopes7/dynatrace-rest-python
 Author: David Lopes
 Author-email: davidribeirolopes@gmail.com
 Project-URL: Issue Tracker, https://github.com/dlopes7/dynatrace-rest-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dt-1.1.59/dt.egg-info/SOURCES.txt` & `dt-1.1.60/dt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 dynatrace/environment_v2/problems.py
 dynatrace/environment_v2/schemas.py
 dynatrace/environment_v2/service_level_objectives.py
 dynatrace/environment_v2/tokens_api.py
 dynatrace/environment_v2/tokens_tenant.py
 test/__init__.py
 test/conftest.py
+test/test_logs.py
 test/configuration_v1/__init__.py
 test/configuration_v1/test_alerting_profiles.py
 test/configuration_v1/test_anomaly_detection_metric_events.py
 test/configuration_v1/test_auto_tags.py
 test/configuration_v1/test_extensions.py
 test/configuration_v1/test_maintenance_windows.py
 test/configuration_v1/test_management_zones.py
```

### Comparing `dt-1.1.59/dynatrace/configuration_v1/alerting_profiles.py` & `dt-1.1.60/dynatrace/configuration_v1/alerting_profiles.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/anomaly_detection_process_groups.py` & `dt-1.1.60/dynatrace/configuration_v1/anomaly_detection_process_groups.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/auto_tags.py` & `dt-1.1.60/dynatrace/configuration_v1/auto_tags.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/credential_vault.py` & `dt-1.1.60/dynatrace/configuration_v1/credential_vault.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/dashboard.py` & `dt-1.1.60/dynatrace/configuration_v1/dashboard.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/endpoint.py` & `dt-1.1.60/dynatrace/configuration_v1/endpoint.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/extensions.py` & `dt-1.1.60/dynatrace/configuration_v1/extensions.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/geographic_regions.py` & `dt-1.1.60/dynatrace/configuration_v1/geographic_regions.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/maintenance_windows.py` & `dt-1.1.60/dynatrace/configuration_v1/maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/management_zones.py` & `dt-1.1.60/dynatrace/configuration_v1/management_zones.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/metric_events.py` & `dt-1.1.60/dynatrace/configuration_v1/metric_events.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/notifications.py` & `dt-1.1.60/dynatrace/configuration_v1/notifications.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/oneagent_environment_wide_configuration.py` & `dt-1.1.60/dynatrace/configuration_v1/oneagent_environment_wide_configuration.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/oneagent_in_a_hostgroup.py` & `dt-1.1.60/dynatrace/configuration_v1/oneagent_in_a_hostgroup.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/oneagent_on_a_host.py` & `dt-1.1.60/dynatrace/configuration_v1/oneagent_on_a_host.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/plugins.py` & `dt-1.1.60/dynatrace/configuration_v1/plugins.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/schemas.py` & `dt-1.1.60/dynatrace/configuration_v1/schemas.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/configuration_v1/tile.py` & `dt-1.1.60/dynatrace/configuration_v1/tile.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/dynatrace_object.py` & `dt-1.1.60/dynatrace/dynatrace_object.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/cluster_time.py` & `dt-1.1.60/dynatrace/environment_v1/cluster_time.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/custom_device.py` & `dt-1.1.60/dynatrace/environment_v1/custom_device.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/deployment.py` & `dt-1.1.60/dynatrace/environment_v1/deployment.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/event.py` & `dt-1.1.60/dynatrace/environment_v1/event.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/oneagents.py` & `dt-1.1.60/dynatrace/environment_v1/oneagents.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/smartscape_hosts.py` & `dt-1.1.60/dynatrace/environment_v1/smartscape_hosts.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/synthetic_monitors.py` & `dt-1.1.60/dynatrace/environment_v1/synthetic_monitors.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/synthetic_third_party.py` & `dt-1.1.60/dynatrace/environment_v1/synthetic_third_party.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v1/timeseries.py` & `dt-1.1.60/dynatrace/environment_v1/timeseries.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/activegates.py` & `dt-1.1.60/dynatrace/environment_v2/activegates.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/activegates_autoupdate_configuration.py` & `dt-1.1.60/dynatrace/environment_v2/activegates_autoupdate_configuration.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/activegates_autoupdate_jobs.py` & `dt-1.1.60/dynatrace/environment_v2/activegates_autoupdate_jobs.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/audit_logs.py` & `dt-1.1.60/dynatrace/environment_v2/audit_logs.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/custom_tags.py` & `dt-1.1.60/dynatrace/environment_v2/custom_tags.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/events.py` & `dt-1.1.60/dynatrace/environment_v2/events.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/extensions.py` & `dt-1.1.60/dynatrace/environment_v2/extensions.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/metrics.py` & `dt-1.1.60/dynatrace/environment_v2/metrics.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/monitored_entities.py` & `dt-1.1.60/dynatrace/environment_v2/monitored_entities.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/networkzones.py` & `dt-1.1.60/dynatrace/environment_v2/networkzones.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/problems.py` & `dt-1.1.60/dynatrace/environment_v2/problems.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/schemas.py` & `dt-1.1.60/dynatrace/environment_v2/schemas.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/service_level_objectives.py` & `dt-1.1.60/dynatrace/environment_v2/service_level_objectives.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/tokens_api.py` & `dt-1.1.60/dynatrace/environment_v2/tokens_api.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/environment_v2/tokens_tenant.py` & `dt-1.1.60/dynatrace/environment_v2/tokens_tenant.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/http_client.py` & `dt-1.1.60/dynatrace/http_client.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/main.py` & `dt-1.1.60/dynatrace/main.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/pagination.py` & `dt-1.1.60/dynatrace/pagination.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/dynatrace/utils.py` & `dt-1.1.60/dynatrace/utils.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/setup.py` & `dt-1.1.60/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="dt",
-    version="1.1.59",
+    version="1.1.60",
     packages=find_packages(),
     install_requires=["requests>=2.22"],
     tests_require=["pytest", "mock", "tox"],
     python_requires=">=3.6",
     author="David Lopes",
     author_email="davidribeirolopes@gmail.com",
     description="Dynatrace API Python client",
```

### Comparing `dt-1.1.59/test/configuration_v1/test_alerting_profiles.py` & `dt-1.1.60/test/configuration_v1/test_alerting_profiles.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_anomaly_detection_metric_events.py` & `dt-1.1.60/test/configuration_v1/test_anomaly_detection_metric_events.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_auto_tags.py` & `dt-1.1.60/test/configuration_v1/test_auto_tags.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_extensions.py` & `dt-1.1.60/test/configuration_v1/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_maintenance_windows.py` & `dt-1.1.60/test/configuration_v1/test_maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_management_zones.py` & `dt-1.1.60/test/configuration_v1/test_management_zones.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_notifications.py` & `dt-1.1.60/test/configuration_v1/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_oneagent_environment_wide_configuration.py` & `dt-1.1.60/test/configuration_v1/test_oneagent_environment_wide_configuration.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_oneagent_in_a_hostgroup.py` & `dt-1.1.60/test/configuration_v1/test_oneagent_in_a_hostgroup.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/configuration_v1/test_oneagent_on_a_host.py` & `dt-1.1.60/test/configuration_v1/test_oneagent_on_a_host.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/conftest.py` & `dt-1.1.60/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v1/test_deployment.py` & `dt-1.1.60/test/environment_v1/test_deployment.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v1/test_smartscape_hosts.py` & `dt-1.1.60/test/environment_v1/test_smartscape_hosts.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v1/test_synthetic_monitors.py` & `dt-1.1.60/test/environment_v1/test_synthetic_monitors.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_activegate_autoupdate_configuration.py` & `dt-1.1.60/test/environment_v2/test_activegate_autoupdate_configuration.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_activegate_autoupdate_jobs.py` & `dt-1.1.60/test/environment_v2/test_activegate_autoupdate_jobs.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_audit_logs.py` & `dt-1.1.60/test/environment_v2/test_audit_logs.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_customtags.py` & `dt-1.1.60/test/environment_v2/test_customtags.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_entities.py` & `dt-1.1.60/test/environment_v2/test_entities.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_events_v2.py` & `dt-1.1.60/test/environment_v2/test_events_v2.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_extensions.py` & `dt-1.1.60/test/environment_v2/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_metrics.py` & `dt-1.1.60/test/environment_v2/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_networkzones.py` & `dt-1.1.60/test/environment_v2/test_networkzones.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_problems.py` & `dt-1.1.60/test/environment_v2/test_problems.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_service_level_objectives.py` & `dt-1.1.60/test/environment_v2/test_service_level_objectives.py`

 * *Files identical despite different names*

### Comparing `dt-1.1.59/test/environment_v2/test_tokens_tenant.py` & `dt-1.1.60/test/environment_v2/test_tokens_tenant.py`

 * *Files identical despite different names*


# Comparing `tmp/benchmark-runner-1.0.98.tar.gz` & `tmp/benchmark-runner-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmark-runner-1.0.98.tar", last modified: Sun Aug  8 05:16:34 2021, max compression
+gzip compressed data, was "benchmark-runner-1.0.99.tar", last modified: Sun Aug  8 07:04:43 2021, max compression
```

## Comparing `benchmark-runner-1.0.98.tar` & `benchmark-runner-1.0.99.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      372 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4495 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.716652 benchmark-runner-1.0.98/benchmark_runner/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.716652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/benchmark_operator_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    26021 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/benchmark_operator_workloads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.716652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.716652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/current_run/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/current_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/generate_yaml_from_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_data_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_pod_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_vm_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ephemeral_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ocs_pvc_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ephemeral_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ocs_pvc_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ephemeral_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ocs_pvc_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_data_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_pod_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_vm_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_data_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_pod_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_vm_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/analyze/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/analyze/analyze_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/clouds/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/clouds/Azure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/clouds/Azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/clouds/Azure/azure_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5638 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/elasticsearch/es_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/logger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/logger/logger_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/oc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14221 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/oc/oc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/oc/oc_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/common/ssh/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/ssh/ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/common/ssh/ssh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/custom_workloads/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/custom_workloads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/benchmark_runner/main/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4782 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3212 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/main/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/benchmark_runner/main/update_data_template_yaml_with_environment_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 05:16:34.716652 benchmark-runner-1.0.98/benchmark_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4495 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-08 05:16:34.000000 benchmark-runner-1.0.98/benchmark_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-08-08 05:16:34.720652 benchmark-runner-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-08-08 05:15:18.000000 benchmark-runner-1.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4495 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.956249 benchmark-runner-1.0.99/benchmark_runner/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.956249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/benchmark_operator_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26021 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/benchmark_operator_workloads.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.956249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/current_run/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/current_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/generate_yaml_from_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_data_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_pod_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_vm_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ephemeral_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ocs_pvc_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ephemeral_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1728 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ocs_pvc_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ephemeral_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2600 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ocs_pvc_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_data_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_pod_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_vm_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_data_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_pod_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_vm_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/analyze/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/analyze/analyze_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/clouds/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/clouds/Azure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/clouds/Azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/clouds/Azure/azure_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5638 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/elasticsearch/es_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/logger/logger_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/oc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14221 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/oc/oc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3688 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/oc/oc_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/common/ssh/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/ssh/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/common/ssh/ssh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/custom_workloads/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/custom_workloads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/benchmark_runner/main/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4782 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/main/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3212 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/main/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-08-08 05:46:34.000000 benchmark-runner-1.0.99/benchmark_runner/main/update_data_template_yaml_with_environment_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 07:04:43.956249 benchmark-runner-1.0.99/benchmark_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4495 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3053 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-08 07:04:43.000000 benchmark-runner-1.0.99/benchmark_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-08-08 07:04:43.960249 benchmark-runner-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-08-08 05:46:35.000000 benchmark-runner-1.0.99/setup.py
```

### Comparing `benchmark-runner-1.0.98/LICENSE` & `benchmark-runner-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/PKG-INFO` & `benchmark-runner-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmark-runner
-Version: 1.0.98
+Version: 1.0.99
 Summary: Benchmark Runner Tool
 Home-page: UNKNOWN
 Author: Red Hat
 Author-email: ebattat@redhat.com
 License: UNKNOWN
 Description: 
         [![Actions Status](https://github.com/redhat-performance/benchmark-runner/workflows/CI/badge.svg)](https://github.com/redhat-performance/benchmark-runner/actions)
```

### Comparing `benchmark-runner-1.0.98/README.md` & `benchmark-runner-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/benchmark_operator_exceptions.py` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/benchmark_operator_exceptions.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/benchmark_operator_workloads.py` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/benchmark_operator_workloads.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/generate_yaml_from_templates.py` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/generate_yaml_from_templates.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_data_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_data_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_pod_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_pod_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_vm_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/hammerdb_vm_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ephemeral_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ephemeral_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ocs_pvc_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mariadb_ocs_pvc_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ephemeral_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ephemeral_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ocs_pvc_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/mssql_ocs_pvc_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ephemeral_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ephemeral_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ocs_pvc_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/hammerdb/postgres_ocs_pvc_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_data_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_data_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_pod_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_pod_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/stressng/stressng_vm_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/stressng/stressng_vm_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_data_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_data_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_pod_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_pod_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/benchmark_operator/templates/uperf/uperf_vm_template.yaml` & `benchmark-runner-1.0.99/benchmark_runner/benchmark_operator/templates/uperf/uperf_vm_template.yaml`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/analyze/analyze_data.py` & `benchmark-runner-1.0.99/benchmark_runner/common/analyze/analyze_data.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/clouds/Azure/azure_operations.py` & `benchmark-runner-1.0.99/benchmark_runner/common/clouds/Azure/azure_operations.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/elasticsearch/es_operations.py` & `benchmark-runner-1.0.99/benchmark_runner/common/elasticsearch/es_operations.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/logger/logger_time_stamp.py` & `benchmark-runner-1.0.99/benchmark_runner/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/oc/oc.py` & `benchmark-runner-1.0.99/benchmark_runner/common/oc/oc.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/oc/oc_exceptions.py` & `benchmark-runner-1.0.99/benchmark_runner/common/oc/oc_exceptions.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/common/ssh/ssh.py` & `benchmark-runner-1.0.99/benchmark_runner/common/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/main/environment_variables.py` & `benchmark-runner-1.0.99/benchmark_runner/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/main/main.py` & `benchmark-runner-1.0.99/benchmark_runner/main/main.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner/main/update_data_template_yaml_with_environment_variables.py` & `benchmark-runner-1.0.99/benchmark_runner/main/update_data_template_yaml_with_environment_variables.py`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/benchmark_runner.egg-info/PKG-INFO` & `benchmark-runner-1.0.99/benchmark_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmark-runner
-Version: 1.0.98
+Version: 1.0.99
 Summary: Benchmark Runner Tool
 Home-page: UNKNOWN
 Author: Red Hat
 Author-email: ebattat@redhat.com
 License: UNKNOWN
 Description: 
         [![Actions Status](https://github.com/redhat-performance/benchmark-runner/workflows/CI/badge.svg)](https://github.com/redhat-performance/benchmark-runner/actions)
```

### Comparing `benchmark-runner-1.0.98/benchmark_runner.egg-info/SOURCES.txt` & `benchmark-runner-1.0.99/benchmark_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benchmark-runner-1.0.98/setup.py` & `benchmark-runner-1.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.98'
+__version__ = '1.0.99'
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
```


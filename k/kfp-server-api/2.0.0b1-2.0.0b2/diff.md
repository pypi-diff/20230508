# Comparing `tmp/kfp-server-api-2.0.0b1.tar.gz` & `tmp/kfp-server-api-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-server-api-2.0.0b1.tar", last modified: Tue Apr 11 20:46:53 2023, max compression
+gzip compressed data, was "kfp-server-api-2.0.0b2.tar", last modified: Mon May  8 16:48:31 2023, max compression
```

## Comparing `kfp-server-api-2.0.0b1.tar` & `kfp-server-api-2.0.0b2.tar`

### file list

```diff
@@ -1,131 +1,188 @@
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11357 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/LICENSE
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      446 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/PKG-INFO
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    13256 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/README.md
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:52.997935 kfp-server-api-2.0.0b1/kfp_server_api/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5053 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/__init__.py
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.001936 kfp-server-api-2.0.0b1/kfp_server_api/api/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      738 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/__init__.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     6214 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/auth_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    36215 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/experiment_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5358 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/healthz_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    57807 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    14031 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_upload_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    37131 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/recurring_run_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11806 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/report_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    54490 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/run_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7057 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/api/visualization_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    26257 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/api_client.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    13316 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/configuration.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3795 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/exceptions.py
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.005936 kfp-server-api-2.0.0b1/kfp_server_api/models/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3959 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/__init__.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2926 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_resources.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2939 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_verb.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5603 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/googlerpc_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4512 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/pipeline_task_detail_child_task.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3379 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_int_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3387 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_long_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3403 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_string_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7241 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_any.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3533 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_list_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2831 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_null_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3522 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_struct.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7513 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2908 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/recurring_run_mode.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3623 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_artifact_list.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4999 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_cron_schedule.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8164 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2999 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment_storage_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3616 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_filter.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3616 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_get_healthz_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5673 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_experiments_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5922 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5687 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipelines_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5803 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5361 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_runs_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5544 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_periodic_schedule.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8024 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    17041 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_detail.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8131 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    11265 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4853 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version_reference.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    10093 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3250 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate_operation.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3903 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_read_artifact_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    19559 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2956 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    18809 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5847 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_details.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2971 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_storage_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4587 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_config.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3157 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4949 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4447 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_trigger.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3547 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_url.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     7294 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2961 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization_type.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)    12327 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/kfp_server_api/rest.py
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:52.997935 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      446 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/PKG-INFO
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5009 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/SOURCES.txt
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)        1 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/dependency_links.txt
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)       48 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/requires.txt
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)       15 2023-04-11 20:46:52.000000 kfp-server-api-2.0.0b1/kfp_server_api.egg-info/top_level.txt
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)       69 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/setup.cfg
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1197 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/setup.py
-drwxr-x---   0 lingqinggan (973760) primarygroup (89939)        0 2023-04-11 20:46:53.013937 kfp-server-api-2.0.0b1/test/
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      849 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_auth_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1511 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_authorize_request_resources.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1456 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_authorize_request_verb.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2074 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_experiment_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1660 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_googlerpc_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      911 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_healthz_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2447 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1600 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_task_detail_child_task.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1043 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_pipeline_upload_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1506 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_int_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1518 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_long_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1540 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_predicate_string_values.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1419 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_protobuf_any.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2787 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_list_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1423 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_protobuf_null_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2235 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_struct.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3325 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_protobuf_value.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1412 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_recurring_run_mode.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2090 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_recurring_run_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      997 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_report_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2416 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_run_service_api.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1524 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_artifact_list.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1686 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_cron_schedule.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1734 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_experiment.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1557 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_experiment_storage_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2288 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_filter.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1547 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_get_healthz_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2140 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_experiments_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3900 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipeline_versions_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2478 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipelines_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     5806 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_recurring_runs_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     8087 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_list_runs_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1741 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_periodic_schedule.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2022 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4402 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_detail.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1863 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_executor_detail.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     3269 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1657 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version_reference.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2265 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_predicate.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1511 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_predicate_operation.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1565 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_read_artifact_response.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     6154 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1513 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     9212 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     4315 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run_details.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1480 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_run_storage_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2870 2023-04-11 20:09:17.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_config.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1445 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_state.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1991 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_status.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     2119 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_trigger.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1379 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_url.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1613 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_visualization.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)     1500 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_v2beta1_visualization_type.py
--rw-r-----   0 lingqinggan (973760) primarygroup (89939)      931 2023-04-11 18:38:21.000000 kfp-server-api-2.0.0b1/test/test_visualization_service_api.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.945034 kfp-server-api-2.0.0b2/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      807 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/.gitignore
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      650 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/.gitlab-ci.yml
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.901030 kfp-server-api-2.0.0b2/.openapi-generator/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)        5 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/.openapi-generator/VERSION
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1040 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/.openapi-generator-ignore
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      344 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/.travis.yml
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    11357 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/LICENSE
+-rw-r-----   0 chesu    (630462) primarygroup (89939)      446 2023-05-08 16:48:31.945034 kfp-server-api-2.0.0b2/PKG-INFO
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    13120 2023-05-08 10:09:52.000000 kfp-server-api-2.0.0b2/README.md
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.917031 kfp-server-api-2.0.0b2/docs/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2838 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/AuthServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      342 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/AuthorizeRequestResources.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      339 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/AuthorizeRequestVerb.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    18273 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/ExperimentServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1273 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/GooglerpcStatus.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2422 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/HealthzServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    28231 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PipelineServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      599 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PipelineTaskDetailChildTask.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5960 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PipelineUploadServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      358 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PredicateIntValues.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      364 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PredicateLongValues.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      360 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/PredicateStringValues.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3964 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/ProtobufAny.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      476 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/ProtobufNullValue.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      511 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/RecurringRunMode.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    18823 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/RecurringRunServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5037 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/ReportServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    26364 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/RunServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      408 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ArtifactList.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      554 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1CronSchedule.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      920 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Experiment.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      498 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ExperimentStorageState.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1128 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Filter.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      379 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1GetHealthzResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      608 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ListExperimentsResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      643 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ListPipelineVersionsResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      647 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ListPipelinesResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      632 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ListRecurringRunsResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      564 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ListRunsResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      690 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PeriodicSchedule.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      964 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Pipeline.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1993 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PipelineTaskDetail.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1222 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PipelineTaskExecutorDetail.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1352 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PipelineVersion.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      555 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PipelineVersionReference.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1137 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Predicate.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      999 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1PredicateOperation.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      376 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1ReadArtifactResponse.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2393 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RecurringRun.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      344 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RecurringRunStatus.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2256 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Run.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      645 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RunDetails.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      491 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RunStorageState.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      526 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RuntimeConfig.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      880 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RuntimeState.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      592 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1RuntimeStatus.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      522 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Trigger.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      371 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Url.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1082 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1Visualization.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      418 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/V2beta1VisualizationType.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2762 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/docs/VisualizationServiceApi.md
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1827 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/git_push.sh
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.917031 kfp-server-api-2.0.0b2/kfp_server_api/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4853 2023-05-08 10:09:52.000000 kfp-server-api-2.0.0b2/kfp_server_api/__init__.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.921032 kfp-server-api-2.0.0b2/kfp_server_api/api/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      738 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/__init__.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6214 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/auth_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    36215 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/experiment_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5358 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/healthz_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    57807 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    14031 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    37131 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/recurring_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    11806 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/report_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    54490 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7057 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/api/visualization_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    26257 2023-05-08 10:09:52.000000 kfp-server-api-2.0.0b2/kfp_server_api/api_client.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    13316 2023-05-08 10:09:52.000000 kfp-server-api-2.0.0b2/kfp_server_api/configuration.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3795 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/exceptions.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.933033 kfp-server-api-2.0.0b2/kfp_server_api/models/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3759 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/__init__.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2926 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/authorize_request_resources.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2939 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/authorize_request_verb.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5603 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/googlerpc_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4512 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/pipeline_task_detail_child_task.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3379 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_int_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3387 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_long_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3403 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_string_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7241 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/protobuf_any.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2831 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/protobuf_null_value.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2908 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/recurring_run_mode.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3623 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_artifact_list.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4999 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_cron_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8164 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_experiment.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2999 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_experiment_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_filter.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_get_healthz_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5673 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_experiments_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5922 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5687 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_pipelines_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5803 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5361 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5544 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_periodic_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8024 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    17041 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_task_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8131 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    11389 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_version.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4853 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_version_reference.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    10093 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_predicate.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3250 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_predicate_operation.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3903 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_read_artifact_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    19617 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_recurring_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2956 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_recurring_run_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    18859 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5847 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run_details.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2971 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4566 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_config.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3157 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4949 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4447 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_trigger.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3547 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_url.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7294 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_visualization.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2961 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_visualization_type.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    12327 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/kfp_server_api/rest.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.917031 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      446 2023-05-08 16:48:30.000000 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6482 2023-05-08 16:48:31.000000 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)        1 2023-05-08 16:48:30.000000 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       48 2023-05-08 16:48:30.000000 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/requires.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       15 2023-05-08 16:48:30.000000 kfp-server-api-2.0.0b2/kfp_server_api.egg-info/top_level.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      126 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/requirements.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       69 2023-05-08 16:48:31.949034 kfp-server-api-2.0.0b2/setup.cfg
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1197 2023-05-08 10:09:52.000000 kfp-server-api-2.0.0b2/setup.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-05-08 16:48:31.945034 kfp-server-api-2.0.0b2/test/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)        0 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/__init__.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      849 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_auth_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_authorize_request_resources.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1456 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_authorize_request_verb.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2074 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_experiment_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1660 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_googlerpc_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      911 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_healthz_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2447 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_pipeline_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1600 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_pipeline_task_detail_child_task.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1043 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1506 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_predicate_int_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1518 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_predicate_long_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1540 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_predicate_string_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1419 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_protobuf_any.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1423 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_protobuf_null_value.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1412 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_recurring_run_mode.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2090 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_recurring_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      997 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_report_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2416 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1524 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_artifact_list.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1686 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_cron_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1734 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_experiment.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1557 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_experiment_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2288 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_filter.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1547 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_get_healthz_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2140 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_list_experiments_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2868 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_list_pipeline_versions_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2478 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_list_pipelines_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4554 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_list_recurring_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6835 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_list_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1741 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_periodic_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2022 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4402 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_task_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1863 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_task_executor_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2357 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_version.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1657 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_version_reference.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2265 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_predicate.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_predicate_operation.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1565 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_read_artifact_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3876 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_recurring_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1513 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_recurring_run_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6934 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4315 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_run_details.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1480 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_run_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1580 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_config.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1445 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1991 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2119 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_trigger.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1379 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_url.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1613 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_visualization.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1500 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_v2beta1_visualization_type.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      931 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test/test_visualization_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      111 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/test-requirements.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      156 2023-05-03 00:12:57.000000 kfp-server-api-2.0.0b2/tox.ini
```

### Comparing `kfp-server-api-2.0.0b1/LICENSE` & `kfp-server-api-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/README.md` & `kfp-server-api-2.0.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kfp-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.0-beta.1
-- Package version: 2.0.0-beta.1
+- API version: 2.0.0-beta.2
+- Package version: 2.0.0-beta.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -142,18 +142,15 @@
  - [AuthorizeRequestVerb](docs/AuthorizeRequestVerb.md)
  - [GooglerpcStatus](docs/GooglerpcStatus.md)
  - [PipelineTaskDetailChildTask](docs/PipelineTaskDetailChildTask.md)
  - [PredicateIntValues](docs/PredicateIntValues.md)
  - [PredicateLongValues](docs/PredicateLongValues.md)
  - [PredicateStringValues](docs/PredicateStringValues.md)
  - [ProtobufAny](docs/ProtobufAny.md)
- - [ProtobufListValue](docs/ProtobufListValue.md)
  - [ProtobufNullValue](docs/ProtobufNullValue.md)
- - [ProtobufStruct](docs/ProtobufStruct.md)
- - [ProtobufValue](docs/ProtobufValue.md)
  - [RecurringRunMode](docs/RecurringRunMode.md)
  - [V2beta1ArtifactList](docs/V2beta1ArtifactList.md)
  - [V2beta1CronSchedule](docs/V2beta1CronSchedule.md)
  - [V2beta1Experiment](docs/V2beta1Experiment.md)
  - [V2beta1ExperimentStorageState](docs/V2beta1ExperimentStorageState.md)
  - [V2beta1Filter](docs/V2beta1Filter.md)
  - [V2beta1GetHealthzResponse](docs/V2beta1GetHealthzResponse.md)
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/__init__.py` & `kfp-server-api-2.0.0b2/kfp_server_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.0.0-beta.1"
+__version__ = "2.0.0-beta.2"
 
 # import apis into sdk package
 from kfp_server_api.api.auth_service_api import AuthServiceApi
 from kfp_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
@@ -40,18 +40,15 @@
 from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb
 from kfp_server_api.models.googlerpc_status import GooglerpcStatus
 from kfp_server_api.models.pipeline_task_detail_child_task import PipelineTaskDetailChildTask
 from kfp_server_api.models.predicate_int_values import PredicateIntValues
 from kfp_server_api.models.predicate_long_values import PredicateLongValues
 from kfp_server_api.models.predicate_string_values import PredicateStringValues
 from kfp_server_api.models.protobuf_any import ProtobufAny
-from kfp_server_api.models.protobuf_list_value import ProtobufListValue
 from kfp_server_api.models.protobuf_null_value import ProtobufNullValue
-from kfp_server_api.models.protobuf_struct import ProtobufStruct
-from kfp_server_api.models.protobuf_value import ProtobufValue
 from kfp_server_api.models.recurring_run_mode import RecurringRunMode
 from kfp_server_api.models.v2beta1_artifact_list import V2beta1ArtifactList
 from kfp_server_api.models.v2beta1_cron_schedule import V2beta1CronSchedule
 from kfp_server_api.models.v2beta1_experiment import V2beta1Experiment
 from kfp_server_api.models.v2beta1_experiment_storage_state import V2beta1ExperimentStorageState
 from kfp_server_api.models.v2beta1_filter import V2beta1Filter
 from kfp_server_api.models.v2beta1_get_healthz_response import V2beta1GetHealthzResponse
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/__init__.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/auth_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/experiment_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/healthz_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/pipeline_upload_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/recurring_run_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/report_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/run_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api/visualization_service_api.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api/visualization_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/api_client.py` & `kfp-server-api-2.0.0b2/kfp_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0-beta.1/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.0-beta.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/configuration.py` & `kfp-server-api-2.0.0b2/kfp_server_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.0-beta.1\n"\
-               "SDK Package Version: 2.0.0-beta.1".\
+               "Version of the API: 2.0.0-beta.2\n"\
+               "SDK Package Version: 2.0.0-beta.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/exceptions.py` & `kfp-server-api-2.0.0b2/kfp_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/__init__.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 from kfp_server_api.models.authorize_request_verb import AuthorizeRequestVerb
 from kfp_server_api.models.googlerpc_status import GooglerpcStatus
 from kfp_server_api.models.pipeline_task_detail_child_task import PipelineTaskDetailChildTask
 from kfp_server_api.models.predicate_int_values import PredicateIntValues
 from kfp_server_api.models.predicate_long_values import PredicateLongValues
 from kfp_server_api.models.predicate_string_values import PredicateStringValues
 from kfp_server_api.models.protobuf_any import ProtobufAny
-from kfp_server_api.models.protobuf_list_value import ProtobufListValue
 from kfp_server_api.models.protobuf_null_value import ProtobufNullValue
-from kfp_server_api.models.protobuf_struct import ProtobufStruct
-from kfp_server_api.models.protobuf_value import ProtobufValue
 from kfp_server_api.models.recurring_run_mode import RecurringRunMode
 from kfp_server_api.models.v2beta1_artifact_list import V2beta1ArtifactList
 from kfp_server_api.models.v2beta1_cron_schedule import V2beta1CronSchedule
 from kfp_server_api.models.v2beta1_experiment import V2beta1Experiment
 from kfp_server_api.models.v2beta1_experiment_storage_state import V2beta1ExperimentStorageState
 from kfp_server_api.models.v2beta1_filter import V2beta1Filter
 from kfp_server_api.models.v2beta1_get_healthz_response import V2beta1GetHealthzResponse
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_resources.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/authorize_request_resources.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/authorize_request_verb.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/authorize_request_verb.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/googlerpc_status.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/pipeline_task_detail_child_task.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/pipeline_task_detail_child_task.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_int_values.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_int_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_long_values.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_long_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/predicate_string_values.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/predicate_string_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_any.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_list_value.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_artifact_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ProtobufListValue(object):
+class V2beta1ArtifactList(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'values': 'list[ProtobufValue]'
+        'artifact_ids': 'list[str]'
     }
 
     attribute_map = {
-        'values': 'values'
+        'artifact_ids': 'artifact_ids'
     }
 
-    def __init__(self, values=None, local_vars_configuration=None):  # noqa: E501
-        """ProtobufListValue - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, artifact_ids=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1ArtifactList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._values = None
+        self._artifact_ids = None
         self.discriminator = None
 
-        if values is not None:
-            self.values = values
+        if artifact_ids is not None:
+            self.artifact_ids = artifact_ids
 
     @property
-    def values(self):
-        """Gets the values of this ProtobufListValue.  # noqa: E501
+    def artifact_ids(self):
+        """Gets the artifact_ids of this V2beta1ArtifactList.  # noqa: E501
 
-        Repeated field of dynamically typed values.  # noqa: E501
+        A list of artifact metadata ids.  # noqa: E501
 
-        :return: The values of this ProtobufListValue.  # noqa: E501
-        :rtype: list[ProtobufValue]
+        :return: The artifact_ids of this V2beta1ArtifactList.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._values
+        return self._artifact_ids
 
-    @values.setter
-    def values(self, values):
-        """Sets the values of this ProtobufListValue.
+    @artifact_ids.setter
+    def artifact_ids(self, artifact_ids):
+        """Sets the artifact_ids of this V2beta1ArtifactList.
 
-        Repeated field of dynamically typed values.  # noqa: E501
+        A list of artifact metadata ids.  # noqa: E501
 
-        :param values: The values of this ProtobufListValue.  # noqa: E501
-        :type values: list[ProtobufValue]
+        :param artifact_ids: The artifact_ids of this V2beta1ArtifactList.  # noqa: E501
+        :type artifact_ids: list[str]
         """
 
-        self._values = values
+        self._artifact_ids = artifact_ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProtobufListValue):
+        if not isinstance(other, V2beta1ArtifactList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProtobufListValue):
+        if not isinstance(other, V2beta1ArtifactList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_null_value.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/protobuf_struct.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_get_healthz_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class ProtobufStruct(object):
+class V2beta1GetHealthzResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'fields': 'dict(str, ProtobufValue)'
+        'multi_user': 'bool'
     }
 
     attribute_map = {
-        'fields': 'fields'
+        'multi_user': 'multi_user'
     }
 
-    def __init__(self, fields=None, local_vars_configuration=None):  # noqa: E501
-        """ProtobufStruct - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, multi_user=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1GetHealthzResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._fields = None
+        self._multi_user = None
         self.discriminator = None
 
-        if fields is not None:
-            self.fields = fields
+        if multi_user is not None:
+            self.multi_user = multi_user
 
     @property
-    def fields(self):
-        """Gets the fields of this ProtobufStruct.  # noqa: E501
+    def multi_user(self):
+        """Gets the multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
 
-        Unordered map of dynamically typed values.  # noqa: E501
+        Returns if KFP in multi-user mode  # noqa: E501
 
-        :return: The fields of this ProtobufStruct.  # noqa: E501
-        :rtype: dict(str, ProtobufValue)
+        :return: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._fields
+        return self._multi_user
 
-    @fields.setter
-    def fields(self, fields):
-        """Sets the fields of this ProtobufStruct.
+    @multi_user.setter
+    def multi_user(self, multi_user):
+        """Sets the multi_user of this V2beta1GetHealthzResponse.
 
-        Unordered map of dynamically typed values.  # noqa: E501
+        Returns if KFP in multi-user mode  # noqa: E501
 
-        :param fields: The fields of this ProtobufStruct.  # noqa: E501
-        :type fields: dict(str, ProtobufValue)
+        :param multi_user: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
+        :type multi_user: bool
         """
 
-        self._fields = fields
+        self._multi_user = multi_user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProtobufStruct):
+        if not isinstance(other, V2beta1GetHealthzResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProtobufStruct):
+        if not isinstance(other, V2beta1GetHealthzResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/recurring_run_mode.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/recurring_run_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_artifact_list.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_url.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1ArtifactList(object):
+class V2beta1Url(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'artifact_ids': 'list[str]'
+        'pipeline_url': 'str'
     }
 
     attribute_map = {
-        'artifact_ids': 'artifact_ids'
+        'pipeline_url': 'pipeline_url'
     }
 
-    def __init__(self, artifact_ids=None, local_vars_configuration=None):  # noqa: E501
-        """V2beta1ArtifactList - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
+        """V2beta1Url - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._artifact_ids = None
+        self._pipeline_url = None
         self.discriminator = None
 
-        if artifact_ids is not None:
-            self.artifact_ids = artifact_ids
+        if pipeline_url is not None:
+            self.pipeline_url = pipeline_url
 
     @property
-    def artifact_ids(self):
-        """Gets the artifact_ids of this V2beta1ArtifactList.  # noqa: E501
+    def pipeline_url(self):
+        """Gets the pipeline_url of this V2beta1Url.  # noqa: E501
 
-        A list of artifact metadata ids.  # noqa: E501
+        URL of the pipeline version definition.  # noqa: E501
 
-        :return: The artifact_ids of this V2beta1ArtifactList.  # noqa: E501
-        :rtype: list[str]
+        :return: The pipeline_url of this V2beta1Url.  # noqa: E501
+        :rtype: str
         """
-        return self._artifact_ids
+        return self._pipeline_url
 
-    @artifact_ids.setter
-    def artifact_ids(self, artifact_ids):
-        """Sets the artifact_ids of this V2beta1ArtifactList.
+    @pipeline_url.setter
+    def pipeline_url(self, pipeline_url):
+        """Sets the pipeline_url of this V2beta1Url.
 
-        A list of artifact metadata ids.  # noqa: E501
+        URL of the pipeline version definition.  # noqa: E501
 
-        :param artifact_ids: The artifact_ids of this V2beta1ArtifactList.  # noqa: E501
-        :type artifact_ids: list[str]
+        :param pipeline_url: The pipeline_url of this V2beta1Url.  # noqa: E501
+        :type pipeline_url: str
         """
 
-        self._artifact_ids = artifact_ids
+        self._pipeline_url = pipeline_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1ArtifactList):
+        if not isinstance(other, V2beta1Url):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1ArtifactList):
+        if not isinstance(other, V2beta1Url):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_cron_schedule.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_experiment_storage_state.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_filter.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_filter.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_get_healthz_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_predicate_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,71 +14,56 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1GetHealthzResponse(object):
+class V2beta1PredicateOperation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    OPERATION_UNSPECIFIED = "OPERATION_UNSPECIFIED"
+    EQUALS = "EQUALS"
+    NOT_EQUALS = "NOT_EQUALS"
+    GREATER_THAN = "GREATER_THAN"
+    GREATER_THAN_EQUALS = "GREATER_THAN_EQUALS"
+    LESS_THAN = "LESS_THAN"
+    LESS_THAN_EQUALS = "LESS_THAN_EQUALS"
+    IN = "IN"
+    IS_SUBSTRING = "IS_SUBSTRING"
+
+    allowable_values = [OPERATION_UNSPECIFIED, EQUALS, NOT_EQUALS, GREATER_THAN, GREATER_THAN_EQUALS, LESS_THAN, LESS_THAN_EQUALS, IN, IS_SUBSTRING]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'multi_user': 'bool'
     }
 
     attribute_map = {
-        'multi_user': 'multi_user'
     }
 
-    def __init__(self, multi_user=None, local_vars_configuration=None):  # noqa: E501
-        """V2beta1GetHealthzResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """V2beta1PredicateOperation - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._multi_user = None
         self.discriminator = None
 
-        if multi_user is not None:
-            self.multi_user = multi_user
-
-    @property
-    def multi_user(self):
-        """Gets the multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-
-        Returns if KFP in multi-user mode  # noqa: E501
-
-        :return: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-        :rtype: bool
-        """
-        return self._multi_user
-
-    @multi_user.setter
-    def multi_user(self, multi_user):
-        """Sets the multi_user of this V2beta1GetHealthzResponse.
-
-        Returns if KFP in multi-user mode  # noqa: E501
-
-        :param multi_user: The multi_user of this V2beta1GetHealthzResponse.  # noqa: E501
-        :type multi_user: bool
-        """
-
-        self._multi_user = multi_user
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -105,18 +90,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1GetHealthzResponse):
+        if not isinstance(other, V2beta1PredicateOperation):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1GetHealthzResponse):
+        if not isinstance(other, V2beta1PredicateOperation):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_experiments_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_pipelines_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_recurring_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_list_runs_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_periodic_schedule.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_task_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'pipeline_id': 'str',
         'pipeline_version_id': 'str',
         'display_name': 'str',
         'description': 'str',
         'created_at': 'datetime',
         'package_url': 'V2beta1Url',
         'code_source_url': 'str',
-        'pipeline_spec': 'ProtobufStruct',
+        'pipeline_spec': 'object',
         'error': 'GooglerpcStatus'
     }
 
     attribute_map = {
         'pipeline_id': 'pipeline_id',
         'pipeline_version_id': 'pipeline_version_id',
         'display_name': 'display_name',
@@ -251,27 +251,29 @@
 
         self._code_source_url = code_source_url
 
     @property
     def pipeline_spec(self):
         """Gets the pipeline_spec of this V2beta1PipelineVersion.  # noqa: E501
 
+        Output. The pipeline spec for the pipeline version.  # noqa: E501
 
         :return: The pipeline_spec of this V2beta1PipelineVersion.  # noqa: E501
-        :rtype: ProtobufStruct
+        :rtype: object
         """
         return self._pipeline_spec
 
     @pipeline_spec.setter
     def pipeline_spec(self, pipeline_spec):
         """Sets the pipeline_spec of this V2beta1PipelineVersion.
 
+        Output. The pipeline spec for the pipeline version.  # noqa: E501
 
         :param pipeline_spec: The pipeline_spec of this V2beta1PipelineVersion.  # noqa: E501
-        :type pipeline_spec: ProtobufStruct
+        :type pipeline_spec: object
         """
 
         self._pipeline_spec = pipeline_spec
 
     @property
     def error(self):
         """Gets the error of this V2beta1PipelineVersion.  # noqa: E501
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_pipeline_version_reference.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_pipeline_version_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_predicate_operation.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_recurring_run_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,35 +14,29 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1PredicateOperation(object):
+class V2beta1RecurringRunStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    OPERATION_UNSPECIFIED = "OPERATION_UNSPECIFIED"
-    EQUALS = "EQUALS"
-    NOT_EQUALS = "NOT_EQUALS"
-    GREATER_THAN = "GREATER_THAN"
-    GREATER_THAN_EQUALS = "GREATER_THAN_EQUALS"
-    LESS_THAN = "LESS_THAN"
-    LESS_THAN_EQUALS = "LESS_THAN_EQUALS"
-    IN = "IN"
-    IS_SUBSTRING = "IS_SUBSTRING"
+    STATUS_UNSPECIFIED = "STATUS_UNSPECIFIED"
+    ENABLED = "ENABLED"
+    DISABLED = "DISABLED"
 
-    allowable_values = [OPERATION_UNSPECIFIED, EQUALS, NOT_EQUALS, GREATER_THAN, GREATER_THAN_EQUALS, LESS_THAN, LESS_THAN_EQUALS, IN, IS_SUBSTRING]  # noqa: E501
+    allowable_values = [STATUS_UNSPECIFIED, ENABLED, DISABLED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -50,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1PredicateOperation - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RecurringRunStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -90,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1PredicateOperation):
+        if not isinstance(other, V2beta1RecurringRunStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1PredicateOperation):
+        if not isinstance(other, V2beta1RecurringRunStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_read_artifact_response.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_recurring_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'recurring_run_id': 'str',
         'display_name': 'str',
         'description': 'str',
         'pipeline_version_id': 'str',
-        'pipeline_spec': 'ProtobufStruct',
+        'pipeline_spec': 'object',
         'pipeline_version_reference': 'V2beta1PipelineVersionReference',
         'runtime_config': 'V2beta1RuntimeConfig',
         'service_account': 'str',
         'max_concurrency': 'str',
         'trigger': 'V2beta1Trigger',
         'mode': 'RecurringRunMode',
         'created_at': 'datetime',
@@ -229,27 +229,29 @@
 
         self._pipeline_version_id = pipeline_version_id
 
     @property
     def pipeline_spec(self):
         """Gets the pipeline_spec of this V2beta1RecurringRun.  # noqa: E501
 
+        The pipeline spec.  # noqa: E501
 
         :return: The pipeline_spec of this V2beta1RecurringRun.  # noqa: E501
-        :rtype: ProtobufStruct
+        :rtype: object
         """
         return self._pipeline_spec
 
     @pipeline_spec.setter
     def pipeline_spec(self, pipeline_spec):
         """Sets the pipeline_spec of this V2beta1RecurringRun.
 
+        The pipeline spec.  # noqa: E501
 
         :param pipeline_spec: The pipeline_spec of this V2beta1RecurringRun.  # noqa: E501
-        :type pipeline_spec: ProtobufStruct
+        :type pipeline_spec: object
         """
 
         self._pipeline_spec = pipeline_spec
 
     @property
     def pipeline_version_reference(self):
         """Gets the pipeline_version_reference of this V2beta1RecurringRun.  # noqa: E501
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_recurring_run_status.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run_storage_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1RecurringRunStatus(object):
+class V2beta1RunStorageState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STATUS_UNSPECIFIED = "STATUS_UNSPECIFIED"
-    ENABLED = "ENABLED"
-    DISABLED = "DISABLED"
+    STORAGE_STATE_UNSPECIFIED = "STORAGE_STATE_UNSPECIFIED"
+    AVAILABLE = "AVAILABLE"
+    ARCHIVED = "ARCHIVED"
 
-    allowable_values = [STATUS_UNSPECIFIED, ENABLED, DISABLED]  # noqa: E501
+    allowable_values = [STORAGE_STATE_UNSPECIFIED, AVAILABLE, ARCHIVED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1RecurringRunStatus - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RunStorageState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1RecurringRunStatus):
+        if not isinstance(other, V2beta1RunStorageState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1RecurringRunStatus):
+        if not isinstance(other, V2beta1RunStorageState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     openapi_types = {
         'experiment_id': 'str',
         'run_id': 'str',
         'display_name': 'str',
         'storage_state': 'V2beta1RunStorageState',
         'description': 'str',
         'pipeline_version_id': 'str',
-        'pipeline_spec': 'ProtobufStruct',
+        'pipeline_spec': 'object',
         'pipeline_version_reference': 'V2beta1PipelineVersionReference',
         'runtime_config': 'V2beta1RuntimeConfig',
         'service_account': 'str',
         'created_at': 'datetime',
         'scheduled_at': 'datetime',
         'finished_at': 'datetime',
         'state': 'V2beta1RuntimeState',
@@ -273,27 +273,29 @@
 
         self._pipeline_version_id = pipeline_version_id
 
     @property
     def pipeline_spec(self):
         """Gets the pipeline_spec of this V2beta1Run.  # noqa: E501
 
+        Pipeline spec.  # noqa: E501
 
         :return: The pipeline_spec of this V2beta1Run.  # noqa: E501
-        :rtype: ProtobufStruct
+        :rtype: object
         """
         return self._pipeline_spec
 
     @pipeline_spec.setter
     def pipeline_spec(self, pipeline_spec):
         """Sets the pipeline_spec of this V2beta1Run.
 
+        Pipeline spec.  # noqa: E501
 
         :param pipeline_spec: The pipeline_spec of this V2beta1Run.  # noqa: E501
-        :type pipeline_spec: ProtobufStruct
+        :type pipeline_spec: object
         """
 
         self._pipeline_spec = pipeline_spec
 
     @property
     def pipeline_version_reference(self):
         """Gets the pipeline_version_reference of this V2beta1Run.  # noqa: E501
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_details.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_run_details.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_run_storage_state.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1RunStorageState(object):
+class V2beta1RuntimeState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STORAGE_STATE_UNSPECIFIED = "STORAGE_STATE_UNSPECIFIED"
-    AVAILABLE = "AVAILABLE"
-    ARCHIVED = "ARCHIVED"
+    RUNTIME_STATE_UNSPECIFIED = "RUNTIME_STATE_UNSPECIFIED"
+    PENDING = "PENDING"
+    RUNNING = "RUNNING"
+    SUCCEEDED = "SUCCEEDED"
+    SKIPPED = "SKIPPED"
+    FAILED = "FAILED"
+    CANCELING = "CANCELING"
+    CANCELED = "CANCELED"
+    PAUSED = "PAUSED"
 
-    allowable_values = [STORAGE_STATE_UNSPECIFIED, AVAILABLE, ARCHIVED]  # noqa: E501
+    allowable_values = [RUNTIME_STATE_UNSPECIFIED, PENDING, RUNNING, SUCCEEDED, SKIPPED, FAILED, CANCELING, CANCELED, PAUSED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +50,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1RunStorageState - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1RuntimeState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +90,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1RunStorageState):
+        if not isinstance(other, V2beta1RuntimeState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1RunStorageState):
+        if not isinstance(other, V2beta1RuntimeState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_config.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'parameters': 'dict(str, ProtobufValue)',
+        'parameters': 'dict(str, object)',
         'pipeline_root': 'str'
     }
 
     attribute_map = {
         'parameters': 'parameters',
         'pipeline_root': 'pipeline_root'
     }
@@ -60,26 +60,26 @@
     @property
     def parameters(self):
         """Gets the parameters of this V2beta1RuntimeConfig.  # noqa: E501
 
         The runtime parameters of the Pipeline. The parameters will be used to replace the placeholders at runtime.  # noqa: E501
 
         :return: The parameters of this V2beta1RuntimeConfig.  # noqa: E501
-        :rtype: dict(str, ProtobufValue)
+        :rtype: dict(str, object)
         """
         return self._parameters
 
     @parameters.setter
     def parameters(self, parameters):
         """Sets the parameters of this V2beta1RuntimeConfig.
 
         The runtime parameters of the Pipeline. The parameters will be used to replace the placeholders at runtime.  # noqa: E501
 
         :param parameters: The parameters of this V2beta1RuntimeConfig.  # noqa: E501
-        :type parameters: dict(str, ProtobufValue)
+        :type parameters: dict(str, object)
         """
 
         self._parameters = parameters
 
     @property
     def pipeline_root(self):
         """Gets the pipeline_root of this V2beta1RuntimeConfig.  # noqa: E501
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_state.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_visualization_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,35 +14,31 @@
 import re  # noqa: F401
 
 import six
 
 from kfp_server_api.configuration import Configuration
 
 
-class V2beta1RuntimeState(object):
+class V2beta1VisualizationType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    RUNTIME_STATE_UNSPECIFIED = "RUNTIME_STATE_UNSPECIFIED"
-    PENDING = "PENDING"
-    RUNNING = "RUNNING"
-    SUCCEEDED = "SUCCEEDED"
-    SKIPPED = "SKIPPED"
-    FAILED = "FAILED"
-    CANCELING = "CANCELING"
-    CANCELED = "CANCELED"
-    PAUSED = "PAUSED"
+    ROC_CURVE = "ROC_CURVE"
+    TFDV = "TFDV"
+    TFMA = "TFMA"
+    TABLE = "TABLE"
+    CUSTOM = "CUSTOM"
 
-    allowable_values = [RUNTIME_STATE_UNSPECIFIED, PENDING, RUNNING, SUCCEEDED, SKIPPED, FAILED, CANCELING, CANCELED, PAUSED]  # noqa: E501
+    allowable_values = [ROC_CURVE, TFDV, TFMA, TABLE, CUSTOM]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -50,15 +46,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V2beta1RuntimeState - a model defined in OpenAPI"""  # noqa: E501
+        """V2beta1VisualizationType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -90,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V2beta1RuntimeState):
+        if not isinstance(other, V2beta1VisualizationType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V2beta1RuntimeState):
+        if not isinstance(other, V2beta1VisualizationType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_runtime_status.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_runtime_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_trigger.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/models/v2beta1_visualization.py` & `kfp-server-api-2.0.0b2/kfp_server_api/models/v2beta1_visualization.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/kfp_server_api/rest.py` & `kfp-server-api-2.0.0b2/kfp_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/setup.py` & `kfp-server-api-2.0.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-server-api"
-VERSION = "2.0.0-beta.1"
+VERSION = "2.0.0-beta.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kfp-server-api-2.0.0b1/test/test_auth_service_api.py` & `kfp-server-api-2.0.0b2/test/test_auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_authorize_request_resources.py` & `kfp-server-api-2.0.0b2/test/test_authorize_request_resources.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_authorize_request_verb.py` & `kfp-server-api-2.0.0b2/test/test_authorize_request_verb.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_experiment_service_api.py` & `kfp-server-api-2.0.0b2/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_googlerpc_status.py` & `kfp-server-api-2.0.0b2/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_healthz_service_api.py` & `kfp-server-api-2.0.0b2/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_pipeline_service_api.py` & `kfp-server-api-2.0.0b2/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_pipeline_task_detail_child_task.py` & `kfp-server-api-2.0.0b2/test/test_pipeline_task_detail_child_task.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_pipeline_upload_service_api.py` & `kfp-server-api-2.0.0b2/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_predicate_int_values.py` & `kfp-server-api-2.0.0b2/test/test_predicate_int_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_predicate_long_values.py` & `kfp-server-api-2.0.0b2/test/test_predicate_long_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_predicate_string_values.py` & `kfp-server-api-2.0.0b2/test/test_predicate_string_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_protobuf_any.py` & `kfp-server-api-2.0.0b2/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_protobuf_null_value.py` & `kfp-server-api-2.0.0b2/test/test_protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_recurring_run_mode.py` & `kfp-server-api-2.0.0b2/test/test_recurring_run_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_recurring_run_service_api.py` & `kfp-server-api-2.0.0b2/test/test_recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_report_service_api.py` & `kfp-server-api-2.0.0b2/test/test_report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_run_service_api.py` & `kfp-server-api-2.0.0b2/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_artifact_list.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_artifact_list.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_cron_schedule.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_experiment.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_experiment_storage_state.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_filter.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_filter.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_get_healthz_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_list_experiments_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_task_detail.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,77 +12,97 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_list_pipeline_versions_response import V2beta1ListPipelineVersionsResponse  # noqa: E501
+from kfp_server_api.models.v2beta1_pipeline_task_detail import V2beta1PipelineTaskDetail  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1ListPipelineVersionsResponse(unittest.TestCase):
-    """V2beta1ListPipelineVersionsResponse unit test stubs"""
+class TestV2beta1PipelineTaskDetail(unittest.TestCase):
+    """V2beta1PipelineTaskDetail unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1ListPipelineVersionsResponse
+        """Test V2beta1PipelineTaskDetail
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_list_pipeline_versions_response.V2beta1ListPipelineVersionsResponse()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_pipeline_task_detail.V2beta1PipelineTaskDetail()  # noqa: E501
         if include_optional :
-            return V2beta1ListPipelineVersionsResponse(
-                pipeline_versions = [
-                    kfp_server_api.models.v2beta1_pipeline_version.v2beta1PipelineVersion(
-                        pipeline_id = '0', 
-                        pipeline_version_id = '0', 
-                        display_name = '0', 
-                        description = '0', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        package_url = kfp_server_api.models.v2beta1_url.v2beta1Url(
-                            pipeline_url = '0', ), 
-                        code_source_url = '0', 
-                        pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
-                            fields = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    null_value = 'NULL_VALUE', 
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, 
-                                    struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(), 
-                                    list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                        values = [
-                                            kfp_server_api.models.protobuf_value.protobufValue(
-                                                number_value = 1.337, 
-                                                string_value = '0', 
-                                                bool_value = True, )
-                                            ], ), )
-                                }, ), 
+            return V2beta1PipelineTaskDetail(
+                run_id = '0', 
+                task_id = '0', 
+                display_name = '0', 
+                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                executor_detail = kfp_server_api.models.v2beta1_pipeline_task_executor_detail.v2beta1PipelineTaskExecutorDetail(
+                    main_job = '0', 
+                    pre_caching_check_job = '0', 
+                    failed_main_jobs = [
+                        '0'
+                        ], 
+                    failed_pre_caching_check_jobs = [
+                        '0'
+                        ], ), 
+                state = 'RUNTIME_STATE_UNSPECIFIED', 
+                execution_id = '0', 
+                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                    code = 56, 
+                    message = '0', 
+                    details = [
+                        kfp_server_api.models.protobuf_any.protobufAny(
+                            type_url = '0', 
+                            value = 'YQ==', )
+                        ], ), 
+                inputs = {
+                    'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
+                        artifact_ids = [
+                            '0'
+                            ], )
+                    }, 
+                outputs = {
+                    'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
+                        artifact_ids = [
+                            '0'
+                            ], )
+                    }, 
+                parent_task_id = '0', 
+                state_history = [
+                    kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
+                        update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        state = 'RUNTIME_STATE_UNSPECIFIED', 
                         error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
                             code = 56, 
                             message = '0', 
                             details = [
                                 kfp_server_api.models.protobuf_any.protobufAny(
                                     type_url = '0', 
                                     value = 'YQ==', )
                                 ], ), )
                     ], 
-                next_page_token = '0', 
-                total_size = 56
+                pod_name = '0', 
+                child_tasks = [
+                    kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                        task_id = '0', 
+                        pod_name = '0', )
+                    ]
             )
         else :
-            return V2beta1ListPipelineVersionsResponse(
+            return V2beta1PipelineTaskDetail(
         )
 
-    def testV2beta1ListPipelineVersionsResponse(self):
-        """Test V2beta1ListPipelineVersionsResponse"""
+    def testV2beta1PipelineTaskDetail(self):
+        """Test V2beta1PipelineTaskDetail"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_list_pipelines_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_list_recurring_runs_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,39 +38,21 @@
             return V2beta1ListRecurringRunsResponse(
                 recurring_runs = [
                     kfp_server_api.models.v2beta1_recurring_run.v2beta1RecurringRun(
                         recurring_run_id = '0', 
                         display_name = '0', 
                         description = '0', 
                         pipeline_version_id = '0', 
-                        pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
-                            fields = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    null_value = 'NULL_VALUE', 
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, 
-                                    struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(), 
-                                    list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                        values = [
-                                            kfp_server_api.models.protobuf_value.protobufValue(
-                                                number_value = 1.337, 
-                                                string_value = '0', 
-                                                bool_value = True, )
-                                            ], ), )
-                                }, ), 
+                        pipeline_spec = kfp_server_api.models.pipeline_spec.pipeline_spec(), 
                         pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
                             pipeline_id = '0', 
                             pipeline_version_id = '0', ), 
                         runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                             parameters = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, )
+                                'key' : None
                                 }, 
                             pipeline_root = '0', ), 
                         service_account = '0', 
                         max_concurrency = '0', 
                         trigger = kfp_server_api.models.v2beta1_trigger.v2beta1Trigger(
                             cron_schedule = kfp_server_api.models.v2beta1_cron_schedule.v2beta1CronSchedule(
                                 start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_list_runs_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_list_runs_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,39 +40,21 @@
                     kfp_server_api.models.v2beta1_run.v2beta1Run(
                         experiment_id = '0', 
                         run_id = '0', 
                         display_name = '0', 
                         storage_state = 'STORAGE_STATE_UNSPECIFIED', 
                         description = '0', 
                         pipeline_version_id = '0', 
-                        pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
-                            fields = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    null_value = 'NULL_VALUE', 
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, 
-                                    struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(), 
-                                    list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                        values = [
-                                            kfp_server_api.models.protobuf_value.protobufValue(
-                                                number_value = 1.337, 
-                                                string_value = '0', 
-                                                bool_value = True, )
-                                            ], ), )
-                                }, ), 
+                        pipeline_spec = kfp_server_api.models.pipeline_spec.pipeline_spec(), 
                         pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
                             pipeline_id = '0', 
                             pipeline_version_id = '0', ), 
                         runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                             parameters = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, )
+                                'key' : None
                                 }, 
                             pipeline_root = '0', ), 
                         service_account = '0', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         scheduled_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         finished_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         state = 'RUNTIME_STATE_UNSPECIFIED',
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_periodic_schedule.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_run_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,97 +12,90 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_pipeline_task_detail import V2beta1PipelineTaskDetail  # noqa: E501
+from kfp_server_api.models.v2beta1_run_details import V2beta1RunDetails  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1PipelineTaskDetail(unittest.TestCase):
-    """V2beta1PipelineTaskDetail unit test stubs"""
+class TestV2beta1RunDetails(unittest.TestCase):
+    """V2beta1RunDetails unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1PipelineTaskDetail
+        """Test V2beta1RunDetails
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_pipeline_task_detail.V2beta1PipelineTaskDetail()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_run_details.V2beta1RunDetails()  # noqa: E501
         if include_optional :
-            return V2beta1PipelineTaskDetail(
-                run_id = '0', 
-                task_id = '0', 
-                display_name = '0', 
-                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                executor_detail = kfp_server_api.models.v2beta1_pipeline_task_executor_detail.v2beta1PipelineTaskExecutorDetail(
-                    main_job = '0', 
-                    pre_caching_check_job = '0', 
-                    failed_main_jobs = [
-                        '0'
-                        ], 
-                    failed_pre_caching_check_jobs = [
-                        '0'
-                        ], ), 
-                state = 'RUNTIME_STATE_UNSPECIFIED', 
-                execution_id = '0', 
-                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
-                    code = 56, 
-                    message = '0', 
-                    details = [
-                        kfp_server_api.models.protobuf_any.protobufAny(
-                            type_url = '0', 
-                            value = 'YQ==', )
-                        ], ), 
-                inputs = {
-                    'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
-                        artifact_ids = [
-                            '0'
-                            ], )
-                    }, 
-                outputs = {
-                    'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
-                        artifact_ids = [
-                            '0'
-                            ], )
-                    }, 
-                parent_task_id = '0', 
-                state_history = [
-                    kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
-                        update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+            return V2beta1RunDetails(
+                pipeline_context_id = '0', 
+                pipeline_run_context_id = '0', 
+                task_details = [
+                    kfp_server_api.models.v2beta1_pipeline_task_detail.v2beta1PipelineTaskDetail(
+                        run_id = '0', 
+                        task_id = '0', 
+                        display_name = '0', 
+                        create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        executor_detail = kfp_server_api.models.v2beta1_pipeline_task_executor_detail.v2beta1PipelineTaskExecutorDetail(
+                            main_job = '0', 
+                            pre_caching_check_job = '0', 
+                            failed_main_jobs = [
+                                '0'
+                                ], 
+                            failed_pre_caching_check_jobs = [
+                                '0'
+                                ], ), 
                         state = 'RUNTIME_STATE_UNSPECIFIED', 
+                        execution_id = '0', 
                         error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
                             code = 56, 
                             message = '0', 
                             details = [
                                 kfp_server_api.models.protobuf_any.protobufAny(
                                     type_url = '0', 
                                     value = 'YQ==', )
-                                ], ), )
-                    ], 
-                pod_name = '0', 
-                child_tasks = [
-                    kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
-                        task_id = '0', 
-                        pod_name = '0', )
+                                ], ), 
+                        inputs = {
+                            'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
+                                artifact_ids = [
+                                    '0'
+                                    ], )
+                            }, 
+                        outputs = {
+                            'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList()
+                            }, 
+                        parent_task_id = '0', 
+                        state_history = [
+                            kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
+                                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                            ], 
+                        pod_name = '0', 
+                        child_tasks = [
+                            kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
+                                task_id = '0', 
+                                pod_name = '0', )
+                            ], )
                     ]
             )
         else :
-            return V2beta1PipelineTaskDetail(
+            return V2beta1RunDetails(
         )
 
-    def testV2beta1PipelineTaskDetail(self):
-        """Test V2beta1PipelineTaskDetail"""
+    def testV2beta1RunDetails(self):
+        """Test V2beta1RunDetails"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_list_pipeline_versions_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,72 +12,62 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_pipeline_version import V2beta1PipelineVersion  # noqa: E501
+from kfp_server_api.models.v2beta1_list_pipeline_versions_response import V2beta1ListPipelineVersionsResponse  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1PipelineVersion(unittest.TestCase):
-    """V2beta1PipelineVersion unit test stubs"""
+class TestV2beta1ListPipelineVersionsResponse(unittest.TestCase):
+    """V2beta1ListPipelineVersionsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1PipelineVersion
+        """Test V2beta1ListPipelineVersionsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_pipeline_version.V2beta1PipelineVersion()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_list_pipeline_versions_response.V2beta1ListPipelineVersionsResponse()  # noqa: E501
         if include_optional :
-            return V2beta1PipelineVersion(
-                pipeline_id = '0', 
-                pipeline_version_id = '0', 
-                display_name = '0', 
-                description = '0', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                package_url = kfp_server_api.models.v2beta1_url.v2beta1Url(
-                    pipeline_url = '0', ), 
-                code_source_url = '0', 
-                pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
-                    fields = {
-                        'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                            null_value = 'NULL_VALUE', 
-                            number_value = 1.337, 
-                            string_value = '0', 
-                            bool_value = True, 
-                            struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(), 
-                            list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                values = [
-                                    kfp_server_api.models.protobuf_value.protobufValue(
-                                        number_value = 1.337, 
-                                        string_value = '0', 
-                                        bool_value = True, )
-                                    ], ), )
-                        }, ), 
-                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
-                    code = 56, 
-                    message = '0', 
-                    details = [
-                        kfp_server_api.models.protobuf_any.protobufAny(
-                            type_url = '0', 
-                            value = 'YQ==', )
-                        ], )
+            return V2beta1ListPipelineVersionsResponse(
+                pipeline_versions = [
+                    kfp_server_api.models.v2beta1_pipeline_version.v2beta1PipelineVersion(
+                        pipeline_id = '0', 
+                        pipeline_version_id = '0', 
+                        display_name = '0', 
+                        description = '0', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        package_url = kfp_server_api.models.v2beta1_url.v2beta1Url(
+                            pipeline_url = '0', ), 
+                        code_source_url = '0', 
+                        pipeline_spec = kfp_server_api.models.pipeline_spec.pipeline_spec(), 
+                        error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                            code = 56, 
+                            message = '0', 
+                            details = [
+                                kfp_server_api.models.protobuf_any.protobufAny(
+                                    type_url = '0', 
+                                    value = 'YQ==', )
+                                ], ), )
+                    ], 
+                next_page_token = '0', 
+                total_size = 56
             )
         else :
-            return V2beta1PipelineVersion(
+            return V2beta1ListPipelineVersionsResponse(
         )
 
-    def testV2beta1PipelineVersion(self):
-        """Test V2beta1PipelineVersion"""
+    def testV2beta1ListPipelineVersionsResponse(self):
+        """Test V2beta1ListPipelineVersionsResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_pipeline_version_reference.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_pipeline_version_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_predicate.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_predicate_operation.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_predicate_operation.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_read_artifact_response.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_recurring_run_status.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_recurring_run_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_run.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,55 +38,21 @@
             return V2beta1Run(
                 experiment_id = '0', 
                 run_id = '0', 
                 display_name = '0', 
                 storage_state = 'STORAGE_STATE_UNSPECIFIED', 
                 description = '0', 
                 pipeline_version_id = '0', 
-                pipeline_spec = kfp_server_api.models.protobuf_struct.protobufStruct(
-                    fields = {
-                        'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                            null_value = 'NULL_VALUE', 
-                            number_value = 1.337, 
-                            string_value = '0', 
-                            bool_value = True, 
-                            struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(), 
-                            list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                values = [
-                                    kfp_server_api.models.protobuf_value.protobufValue(
-                                        number_value = 1.337, 
-                                        string_value = '0', 
-                                        bool_value = True, )
-                                    ], ), )
-                        }, ), 
+                pipeline_spec = kfp_server_api.models.pipeline_spec.pipeline_spec(), 
                 pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
                     pipeline_id = '0', 
                     pipeline_version_id = '0', ), 
                 runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
                     parameters = {
-                        'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                            null_value = 'NULL_VALUE', 
-                            number_value = 1.337, 
-                            string_value = '0', 
-                            bool_value = True, 
-                            struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(
-                                fields = {
-                                    'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                        number_value = 1.337, 
-                                        string_value = '0', 
-                                        bool_value = True, 
-                                        list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                            values = [
-                                                kfp_server_api.models.protobuf_value.protobufValue(
-                                                    number_value = 1.337, 
-                                                    string_value = '0', 
-                                                    bool_value = True, )
-                                                ], ), )
-                                    }, ), 
-                            list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(), )
+                        'key' : None
                         }, 
                     pipeline_root = '0', ), 
                 service_account = '0', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 scheduled_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 finished_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 state = 'RUNTIME_STATE_UNSPECIFIED',
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_run_details.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_recurring_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,90 +12,79 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_run_details import V2beta1RunDetails  # noqa: E501
+from kfp_server_api.models.v2beta1_recurring_run import V2beta1RecurringRun  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1RunDetails(unittest.TestCase):
-    """V2beta1RunDetails unit test stubs"""
+class TestV2beta1RecurringRun(unittest.TestCase):
+    """V2beta1RecurringRun unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1RunDetails
+        """Test V2beta1RecurringRun
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_run_details.V2beta1RunDetails()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_recurring_run.V2beta1RecurringRun()  # noqa: E501
         if include_optional :
-            return V2beta1RunDetails(
-                pipeline_context_id = '0', 
-                pipeline_run_context_id = '0', 
-                task_details = [
-                    kfp_server_api.models.v2beta1_pipeline_task_detail.v2beta1PipelineTaskDetail(
-                        run_id = '0', 
-                        task_id = '0', 
-                        display_name = '0', 
-                        create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+            return V2beta1RecurringRun(
+                recurring_run_id = '0', 
+                display_name = '0', 
+                description = '0', 
+                pipeline_version_id = '0', 
+                pipeline_spec = kfp_server_api.models.pipeline_spec.pipeline_spec(), 
+                pipeline_version_reference = kfp_server_api.models.v2beta1_pipeline_version_reference.v2beta1PipelineVersionReference(
+                    pipeline_id = '0', 
+                    pipeline_version_id = '0', ), 
+                runtime_config = kfp_server_api.models.v2beta1_runtime_config.v2beta1RuntimeConfig(
+                    parameters = {
+                        'key' : None
+                        }, 
+                    pipeline_root = '0', ), 
+                service_account = '0', 
+                max_concurrency = '0', 
+                trigger = kfp_server_api.models.v2beta1_trigger.v2beta1Trigger(
+                    cron_schedule = kfp_server_api.models.v2beta1_cron_schedule.v2beta1CronSchedule(
                         start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        executor_detail = kfp_server_api.models.v2beta1_pipeline_task_executor_detail.v2beta1PipelineTaskExecutorDetail(
-                            main_job = '0', 
-                            pre_caching_check_job = '0', 
-                            failed_main_jobs = [
-                                '0'
-                                ], 
-                            failed_pre_caching_check_jobs = [
-                                '0'
-                                ], ), 
-                        state = 'RUNTIME_STATE_UNSPECIFIED', 
-                        execution_id = '0', 
-                        error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
-                            code = 56, 
-                            message = '0', 
-                            details = [
-                                kfp_server_api.models.protobuf_any.protobufAny(
-                                    type_url = '0', 
-                                    value = 'YQ==', )
-                                ], ), 
-                        inputs = {
-                            'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList(
-                                artifact_ids = [
-                                    '0'
-                                    ], )
-                            }, 
-                        outputs = {
-                            'key' : kfp_server_api.models.v2beta1_artifact_list.v2beta1ArtifactList()
-                            }, 
-                        parent_task_id = '0', 
-                        state_history = [
-                            kfp_server_api.models.v2beta1_runtime_status.v2beta1RuntimeStatus(
-                                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
-                            ], 
-                        pod_name = '0', 
-                        child_tasks = [
-                            kfp_server_api.models.pipeline_task_detail_child_task.PipelineTaskDetailChildTask(
-                                task_id = '0', 
-                                pod_name = '0', )
-                            ], )
-                    ]
+                        cron = '0', ), 
+                    periodic_schedule = kfp_server_api.models.v2beta1_periodic_schedule.v2beta1PeriodicSchedule(
+                        start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        interval_second = '0', ), ), 
+                mode = 'MODE_UNSPECIFIED', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                status = 'STATUS_UNSPECIFIED', 
+                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                    code = 56, 
+                    message = '0', 
+                    details = [
+                        kfp_server_api.models.protobuf_any.protobufAny(
+                            type_url = '0', 
+                            value = 'YQ==', )
+                        ], ), 
+                no_catchup = True, 
+                namespace = '0', 
+                experiment_id = '0'
             )
         else :
-            return V2beta1RunDetails(
+            return V2beta1RecurringRun(
         )
 
-    def testV2beta1RunDetails(self):
-        """Test V2beta1RunDetails"""
+    def testV2beta1RecurringRun(self):
+        """Test V2beta1RecurringRun"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_run_storage_state.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_config.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,63 +12,50 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_runtime_config import V2beta1RuntimeConfig  # noqa: E501
+from kfp_server_api.models.v2beta1_runtime_status import V2beta1RuntimeStatus  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1RuntimeConfig(unittest.TestCase):
-    """V2beta1RuntimeConfig unit test stubs"""
+class TestV2beta1RuntimeStatus(unittest.TestCase):
+    """V2beta1RuntimeStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1RuntimeConfig
+        """Test V2beta1RuntimeStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_runtime_config.V2beta1RuntimeConfig()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_runtime_status.V2beta1RuntimeStatus()  # noqa: E501
         if include_optional :
-            return V2beta1RuntimeConfig(
-                parameters = {
-                    'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                        null_value = 'NULL_VALUE', 
-                        number_value = 1.337, 
-                        string_value = '0', 
-                        bool_value = True, 
-                        struct_value = kfp_server_api.models.protobuf_struct.protobufStruct(
-                            fields = {
-                                'key' : kfp_server_api.models.protobuf_value.protobufValue(
-                                    number_value = 1.337, 
-                                    string_value = '0', 
-                                    bool_value = True, 
-                                    list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(
-                                        values = [
-                                            kfp_server_api.models.protobuf_value.protobufValue(
-                                                number_value = 1.337, 
-                                                string_value = '0', 
-                                                bool_value = True, )
-                                            ], ), )
-                                }, ), 
-                        list_value = kfp_server_api.models.protobuf_list_value.protobufListValue(), )
-                    }, 
-                pipeline_root = '0'
+            return V2beta1RuntimeStatus(
+                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                state = 'RUNTIME_STATE_UNSPECIFIED', 
+                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
+                    code = 56, 
+                    message = '0', 
+                    details = [
+                        kfp_server_api.models.protobuf_any.protobufAny(
+                            type_url = '0', 
+                            value = 'YQ==', )
+                        ], )
             )
         else :
-            return V2beta1RuntimeConfig(
+            return V2beta1RuntimeStatus(
         )
 
-    def testV2beta1RuntimeConfig(self):
-        """Test V2beta1RuntimeConfig"""
+    def testV2beta1RuntimeStatus(self):
+        """Test V2beta1RuntimeStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_state.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_runtime_status.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_runtime_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,50 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_server_api
-from kfp_server_api.models.v2beta1_runtime_status import V2beta1RuntimeStatus  # noqa: E501
+from kfp_server_api.models.v2beta1_runtime_config import V2beta1RuntimeConfig  # noqa: E501
 from kfp_server_api.rest import ApiException
 
-class TestV2beta1RuntimeStatus(unittest.TestCase):
-    """V2beta1RuntimeStatus unit test stubs"""
+class TestV2beta1RuntimeConfig(unittest.TestCase):
+    """V2beta1RuntimeConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V2beta1RuntimeStatus
+        """Test V2beta1RuntimeConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_server_api.models.v2beta1_runtime_status.V2beta1RuntimeStatus()  # noqa: E501
+        # model = kfp_server_api.models.v2beta1_runtime_config.V2beta1RuntimeConfig()  # noqa: E501
         if include_optional :
-            return V2beta1RuntimeStatus(
-                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                state = 'RUNTIME_STATE_UNSPECIFIED', 
-                error = kfp_server_api.models.googlerpc_status.googlerpcStatus(
-                    code = 56, 
-                    message = '0', 
-                    details = [
-                        kfp_server_api.models.protobuf_any.protobufAny(
-                            type_url = '0', 
-                            value = 'YQ==', )
-                        ], )
+            return V2beta1RuntimeConfig(
+                parameters = {
+                    'key' : None
+                    }, 
+                pipeline_root = '0'
             )
         else :
-            return V2beta1RuntimeStatus(
+            return V2beta1RuntimeConfig(
         )
 
-    def testV2beta1RuntimeStatus(self):
-        """Test V2beta1RuntimeStatus"""
+    def testV2beta1RuntimeConfig(self):
+        """Test V2beta1RuntimeConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_trigger.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_url.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_visualization.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_visualization.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_v2beta1_visualization_type.py` & `kfp-server-api-2.0.0b2/test/test_v2beta1_visualization_type.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.0.0b1/test/test_visualization_service_api.py` & `kfp-server-api-2.0.0b2/test/test_visualization_service_api.py`

 * *Files identical despite different names*


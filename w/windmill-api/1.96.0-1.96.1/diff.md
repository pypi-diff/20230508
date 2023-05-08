# Comparing `tmp/windmill_api-1.96.0.tar.gz` & `tmp/windmill_api-1.96.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.96.0.tar", max compression
+gzip compressed data, was "windmill_api-1.96.1.tar", max compression
```

## Comparing `windmill_api-1.96.0.tar` & `windmill_api-1.96.1.tar`

### file list

```diff
@@ -1,1302 +1,1302 @@
--rw-r--r--   0        0        0    11348 2023-05-08 17:45:53.465227 windmill_api-1.96.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-08 17:45:53.473228 windmill_api-1.96.0/README.md
--rw-r--r--   0        0        0      717 2023-05-08 17:45:53.465227 windmill_api-1.96.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-08 17:45:08.361165 windmill_api-1.96.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-08 17:45:09.081166 windmill_api-1.96.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.253166 windmill_api-1.96.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-08 17:45:22.989157 windmill_api-1.96.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-08 17:45:23.049157 windmill_api-1.96.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-08 17:45:23.041157 windmill_api-1.96.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-08 17:45:23.089157 windmill_api-1.96.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-08 17:45:23.125157 windmill_api-1.96.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-08 17:45:23.141157 windmill_api-1.96.0/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-08 17:45:23.181158 windmill_api-1.96.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-08 17:45:23.209158 windmill_api-1.96.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-08 17:45:23.261158 windmill_api-1.96.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-08 17:45:23.249158 windmill_api-1.96.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-08 17:45:23.369158 windmill_api-1.96.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-08 17:45:23.309158 windmill_api-1.96.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-08 17:45:23.361158 windmill_api-1.96.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.133165 windmill_api-1.96.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-08 17:45:23.417158 windmill_api-1.96.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-08 17:45:23.521159 windmill_api-1.96.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.341166 windmill_api-1.96.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-08 17:45:23.453159 windmill_api-1.96.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-08 17:45:23.501159 windmill_api-1.96.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-08 17:45:23.537159 windmill_api-1.96.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.265166 windmill_api-1.96.0/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-08 17:45:23.569159 windmill_api-1.96.0/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.345166 windmill_api-1.96.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-08 17:45:23.577159 windmill_api-1.96.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-08 17:45:23.613159 windmill_api-1.96.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.221166 windmill_api-1.96.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-08 17:45:23.621159 windmill_api-1.96.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-08 17:45:23.681159 windmill_api-1.96.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-08 17:45:23.661159 windmill_api-1.96.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-08 17:45:23.713160 windmill_api-1.96.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-08 17:45:23.737160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-08 17:45:23.785160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-08 17:45:23.825160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-08 17:45:23.833160 windmill_api-1.96.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-08 17:45:23.869160 windmill_api-1.96.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-08 17:45:23.969160 windmill_api-1.96.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-08 17:45:23.917160 windmill_api-1.96.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-08 17:45:23.965160 windmill_api-1.96.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.329166 windmill_api-1.96.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-08 17:45:24.013161 windmill_api-1.96.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-08 17:45:24.009161 windmill_api-1.96.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-08 17:45:24.049161 windmill_api-1.96.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-08 17:45:24.073161 windmill_api-1.96.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-08 17:45:24.113161 windmill_api-1.96.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-08 17:45:24.145161 windmill_api-1.96.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-08 17:45:24.197161 windmill_api-1.96.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-08 17:45:24.217162 windmill_api-1.96.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-08 17:45:24.261162 windmill_api-1.96.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.337165 windmill_api-1.96.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-08 17:45:24.273162 windmill_api-1.96.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-08 17:45:24.321162 windmill_api-1.96.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-08 17:45:24.317162 windmill_api-1.96.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.321166 windmill_api-1.96.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-08 17:45:24.365162 windmill_api-1.96.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-08 17:45:24.361162 windmill_api-1.96.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-08 17:45:24.397162 windmill_api-1.96.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-08 17:45:24.425162 windmill_api-1.96.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-08 17:45:24.477162 windmill_api-1.96.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-08 17:45:24.509163 windmill_api-1.96.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-08 17:45:24.521163 windmill_api-1.96.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-08 17:45:24.553163 windmill_api-1.96.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.345166 windmill_api-1.96.0/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-08 17:45:24.581163 windmill_api-1.96.0/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-08 17:45:24.597163 windmill_api-1.96.0/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-08 17:45:24.693163 windmill_api-1.96.0/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-08 17:45:24.713163 windmill_api-1.96.0/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-08 17:45:24.753163 windmill_api-1.96.0/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.269166 windmill_api-1.96.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-08 17:45:24.761163 windmill_api-1.96.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-08 17:45:24.809163 windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 17:45:24.817164 windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-08 17:45:24.861164 windmill_api-1.96.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-08 17:45:24.877164 windmill_api-1.96.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-08 17:45:24.901164 windmill_api-1.96.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-08 17:45:24.933164 windmill_api-1.96.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:24.941164 windmill_api-1.96.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-08 17:45:24.985164 windmill_api-1.96.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-08 17:45:25.021164 windmill_api-1.96.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-08 17:45:25.057165 windmill_api-1.96.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-08 17:45:25.097164 windmill_api-1.96.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-08 17:45:25.277165 windmill_api-1.96.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-08 17:45:25.317165 windmill_api-1.96.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-08 17:45:25.485166 windmill_api-1.96.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-08 17:45:25.361166 windmill_api-1.96.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-08 17:45:25.405166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-08 17:45:25.461166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 17:45:25.517166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-08 17:45:25.565166 windmill_api-1.96.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-08 17:45:25.569166 windmill_api-1.96.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-08 17:45:25.673167 windmill_api-1.96.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-08 17:45:25.641167 windmill_api-1.96.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-08 17:45:25.717167 windmill_api-1.96.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-08 17:45:25.725167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-08 17:45:25.777167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-08 17:45:25.793167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.177166 windmill_api-1.96.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-08 17:45:25.833167 windmill_api-1.96.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-08 17:45:25.833167 windmill_api-1.96.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-08 17:45:25.877167 windmill_api-1.96.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-08 17:45:25.873167 windmill_api-1.96.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-08 17:45:25.913168 windmill_api-1.96.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-08 17:45:25.905167 windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-08 17:45:25.953168 windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-08 17:45:25.953168 windmill_api-1.96.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.305166 windmill_api-1.96.0/windmill_api/api/raw_app/__init__.py
--rw-r--r--   0        0        0     2033 2023-05-08 17:45:25.997168 windmill_api-1.96.0/windmill_api/api/raw_app/create_raw_app.py
--rw-r--r--   0        0        0     1781 2023-05-08 17:45:25.997168 windmill_api-1.96.0/windmill_api/api/raw_app/delete_raw_app.py
--rw-r--r--   0        0        0     2786 2023-05-08 17:45:26.045168 windmill_api-1.96.0/windmill_api/api/raw_app/exists_raw_app.py
--rw-r--r--   0        0        0     1979 2023-05-08 17:45:26.037168 windmill_api-1.96.0/windmill_api/api/raw_app/get_raw_app_data.py
--rw-r--r--   0        0        0     7349 2023-05-08 17:45:26.177168 windmill_api-1.96.0/windmill_api/api/raw_app/list_raw_apps.py
--rw-r--r--   0        0        0     2166 2023-05-08 17:45:26.089168 windmill_api-1.96.0/windmill_api/api/raw_app/update_raw_app.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.185166 windmill_api-1.96.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 17:45:26.129168 windmill_api-1.96.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-08 17:45:26.189169 windmill_api-1.96.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:26.217169 windmill_api-1.96.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-08 17:45:26.225169 windmill_api-1.96.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-08 17:45:26.273169 windmill_api-1.96.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-08 17:45:26.289169 windmill_api-1.96.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-08 17:45:26.333169 windmill_api-1.96.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-08 17:45:26.349169 windmill_api-1.96.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-08 17:45:26.377169 windmill_api-1.96.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-08 17:45:26.449169 windmill_api-1.96.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-08 17:45:26.437169 windmill_api-1.96.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-08 17:45:26.497170 windmill_api-1.96.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-08 17:45:26.489170 windmill_api-1.96.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-08 17:45:26.541170 windmill_api-1.96.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-08 17:45:26.545170 windmill_api-1.96.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.313166 windmill_api-1.96.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 17:45:26.581170 windmill_api-1.96.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:26.589170 windmill_api-1.96.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-08 17:45:26.649170 windmill_api-1.96.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-08 17:45:26.669170 windmill_api-1.96.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-08 17:45:26.761170 windmill_api-1.96.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-08 17:45:26.725170 windmill_api-1.96.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-08 17:45:26.777171 windmill_api-1.96.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-08 17:45:26.805171 windmill_api-1.96.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.201166 windmill_api-1.96.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-08 17:45:26.841171 windmill_api-1.96.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-08 17:45:26.845171 windmill_api-1.96.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 17:45:26.905171 windmill_api-1.96.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-08 17:45:26.889171 windmill_api-1.96.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-08 17:45:26.945171 windmill_api-1.96.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-08 17:45:26.969171 windmill_api-1.96.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 17:45:27.001171 windmill_api-1.96.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-08 17:45:27.025172 windmill_api-1.96.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-08 17:45:27.053172 windmill_api-1.96.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-08 17:45:27.065172 windmill_api-1.96.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-08 17:45:27.117172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-08 17:45:27.125172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-08 17:45:27.197172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-08 17:45:27.201172 windmill_api-1.96.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-08 17:45:27.249172 windmill_api-1.96.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-08 17:45:27.253172 windmill_api-1.96.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-08 17:45:27.285173 windmill_api-1.96.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-08 17:45:27.445173 windmill_api-1.96.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-08 17:45:27.345173 windmill_api-1.96.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:27.381173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:27.425173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-08 17:45:27.473173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.101166 windmill_api-1.96.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-08 17:45:27.481173 windmill_api-1.96.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-08 17:45:27.513173 windmill_api-1.96.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.137166 windmill_api-1.96.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-08 17:45:27.541173 windmill_api-1.96.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-08 17:45:27.549173 windmill_api-1.96.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-08 17:45:27.577174 windmill_api-1.96.0/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-08 17:45:27.589174 windmill_api-1.96.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-08 17:45:27.617174 windmill_api-1.96.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-08 17:45:27.629174 windmill_api-1.96.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-08 17:45:27.653174 windmill_api-1.96.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-08 17:45:27.681174 windmill_api-1.96.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-08 17:45:27.713174 windmill_api-1.96.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-08 17:45:27.717174 windmill_api-1.96.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-08 17:45:27.753174 windmill_api-1.96.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-08 17:45:27.757174 windmill_api-1.96.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-08 17:45:27.797174 windmill_api-1.96.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-08 17:45:27.805174 windmill_api-1.96.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-08 17:45:27.833175 windmill_api-1.96.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-08 17:45:27.861175 windmill_api-1.96.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-08 17:45:27.889175 windmill_api-1.96.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-08 17:45:27.945175 windmill_api-1.96.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-08 17:45:27.973175 windmill_api-1.96.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-08 17:45:28.001175 windmill_api-1.96.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:28.013175 windmill_api-1.96.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-08 17:45:28.041175 windmill_api-1.96.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-08 17:45:28.053175 windmill_api-1.96.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-08 17:45:28.081175 windmill_api-1.96.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-08 17:45:28.101175 windmill_api-1.96.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-08 17:45:28.133175 windmill_api-1.96.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-08 17:45:28.157176 windmill_api-1.96.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.173166 windmill_api-1.96.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-08 17:45:28.193176 windmill_api-1.96.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-08 17:45:28.209176 windmill_api-1.96.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-08 17:45:28.249176 windmill_api-1.96.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-08 17:45:28.277176 windmill_api-1.96.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-08 17:45:28.305176 windmill_api-1.96.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-08 17:45:28.333176 windmill_api-1.96.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-08 17:45:28.357176 windmill_api-1.96.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.265166 windmill_api-1.96.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-08 17:45:28.381176 windmill_api-1.96.0/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-08 17:45:28.429176 windmill_api-1.96.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-08 17:45:09.157166 windmill_api-1.96.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-08 17:45:28.425176 windmill_api-1.96.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-08 17:45:28.457176 windmill_api-1.96.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.465176 windmill_api-1.96.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-08 17:45:28.497176 windmill_api-1.96.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-08 17:45:28.505176 windmill_api-1.96.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-08 17:45:28.549177 windmill_api-1.96.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-08 17:45:28.545176 windmill_api-1.96.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-08 17:45:28.589177 windmill_api-1.96.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.601177 windmill_api-1.96.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.649177 windmill_api-1.96.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-08 17:45:28.657177 windmill_api-1.96.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-08 17:45:28.705177 windmill_api-1.96.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-08 17:45:28.717177 windmill_api-1.96.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-08 17:45:28.757177 windmill_api-1.96.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-08 17:45:28.777177 windmill_api-1.96.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-08 17:45:28.805177 windmill_api-1.96.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-08 17:45:28.829177 windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-08 17:45:28.885177 windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-08 17:45:28.873177 windmill_api-1.96.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-08 17:45:28.917177 windmill_api-1.96.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-08 17:45:53.457228 windmill_api-1.96.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-08 17:45:28.953177 windmill_api-1.96.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-08 17:45:28.989177 windmill_api-1.96.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      325 2023-05-08 17:45:20.973151 windmill_api-1.96.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-08 17:45:29.025177 windmill_api-1.96.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-08 17:45:29.073177 windmill_api-1.96.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-08 17:45:29.109177 windmill_api-1.96.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-08 17:45:29.185178 windmill_api-1.96.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-08 17:45:21.713152 windmill_api-1.96.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-08 17:45:29.137178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-08 17:45:29.233178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-08 17:45:21.781153 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-08 17:45:29.229178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-08 17:45:29.261178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-08 17:45:29.309178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-08 17:45:29.289178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-08 17:45:29.365178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-08 17:45:21.145151 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-08 17:45:29.345178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-08 17:45:29.373178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-08 17:45:29.409178 windmill_api-1.96.0/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-08 17:45:29.509178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-08 17:45:29.433178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-08 17:45:22.105154 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-08 17:45:21.665152 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-08 17:45:29.481178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-08 17:45:29.569178 windmill_api-1.96.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-08 17:45:21.765153 windmill_api-1.96.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-08 17:45:21.601152 windmill_api-1.96.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-08 17:45:29.545178 windmill_api-1.96.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-08 17:45:29.601179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 17:45:29.665179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 17:45:21.625152 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 17:45:29.633179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 17:45:29.669179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 17:45:29.741179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 17:45:29.749179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 17:45:21.861153 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 17:45:29.785179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 17:45:29.813179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 17:45:21.781153 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 17:45:29.821179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 17:45:20.753150 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 17:45:29.865179 windmill_api-1.96.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-08 17:45:29.869179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 17:45:29.985179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 17:45:29.921179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 17:45:29.961179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 17:45:30.009179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 17:45:30.029179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:21.737152 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 17:45:30.053179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:21.165151 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 17:45:30.077179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 17:45:30.093179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 17:45:21.045151 windmill_api-1.96.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-08 17:45:30.133180 windmill_api-1.96.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-08 17:45:30.141179 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 17:45:30.289180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 17:45:30.205180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 17:45:30.261180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 17:45:30.305180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 17:45:30.333180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:21.609152 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 17:45:30.345180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:20.949151 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 17:45:30.381180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 17:45:30.389180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 17:45:30.513180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 17:45:30.445180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 17:45:30.489180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 17:45:30.537180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 17:45:30.557180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 17:45:30.581180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 17:45:21.973153 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 17:45:30.609180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 17:45:30.629180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 17:45:21.749153 windmill_api-1.96.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-08 17:45:30.657180 windmill_api-1.96.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 17:45:30.657180 windmill_api-1.96.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-08 17:45:30.897181 windmill_api-1.96.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-08 17:45:30.689180 windmill_api-1.96.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 17:45:30.749181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-08 17:45:30.889181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-08 17:45:30.929181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-08 17:45:30.945181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-08 17:45:21.997153 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-08 17:45:30.969181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-08 17:45:31.005181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-08 17:45:20.921151 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-08 17:45:31.121181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-08 17:45:31.041181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 17:45:31.093181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-08 17:45:20.593150 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-08 17:45:31.137181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-08 17:45:31.169181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-08 17:45:22.105154 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-08 17:45:31.193181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-08 17:45:21.281151 windmill_api-1.96.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-08 17:45:20.577150 windmill_api-1.96.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-08 17:45:31.237182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-08 17:45:31.313182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-08 17:45:31.293182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 17:45:31.357182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 17:45:31.365182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 17:45:31.393182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:21.413152 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 17:45:31.405182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:21.405151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 17:45:31.433182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 17:45:31.469182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-08 17:45:31.537182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-08 17:45:31.521182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-08 17:45:31.561182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-08 17:45:31.577182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-08 17:45:31.601182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-08 17:45:21.117151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-08 17:45:31.609182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-08 17:45:21.173151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-08 17:45:31.641182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-08 17:45:31.649182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-08 17:45:31.681182 windmill_api-1.96.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-08 17:45:31.697182 windmill_api-1.96.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-08 17:45:31.717182 windmill_api-1.96.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-08 17:45:31.737182 windmill_api-1.96.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-08 17:45:31.769183 windmill_api-1.96.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-08 17:45:31.785183 windmill_api-1.96.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 17:45:31.833183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:22.117154 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 17:45:31.837183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 17:45:31.861183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-08 17:45:31.881183 windmill_api-1.96.0/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-08 17:45:21.341151 windmill_api-1.96.0/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-08 17:45:31.901183 windmill_api-1.96.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-08 17:45:31.925183 windmill_api-1.96.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-08 17:45:31.941183 windmill_api-1.96.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-08 17:45:31.965183 windmill_api-1.96.0/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-08 17:45:31.997183 windmill_api-1.96.0/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-08 17:45:31.997183 windmill_api-1.96.0/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-08 17:45:32.029183 windmill_api-1.96.0/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-08 17:45:20.617150 windmill_api-1.96.0/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     1732 2023-05-08 17:45:32.037183 windmill_api-1.96.0/windmill_api/models/create_raw_app_json_body.py
--rw-r--r--   0        0        0     2094 2023-05-08 17:45:32.073183 windmill_api-1.96.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-08 17:45:32.081183 windmill_api-1.96.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-08 17:45:32.125183 windmill_api-1.96.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-08 17:45:32.137183 windmill_api-1.96.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:32.149183 windmill_api-1.96.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-08 17:45:32.237183 windmill_api-1.96.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-08 17:45:22.113154 windmill_api-1.96.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-08 17:45:20.581150 windmill_api-1.96.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:32.189183 windmill_api-1.96.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-08 17:45:32.241183 windmill_api-1.96.0/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-08 17:45:32.281183 windmill_api-1.96.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-08 17:45:32.297183 windmill_api-1.96.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-08 17:45:32.341184 windmill_api-1.96.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-08 17:45:32.349184 windmill_api-1.96.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-08 17:45:32.389184 windmill_api-1.96.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-08 17:45:32.385184 windmill_api-1.96.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-08 17:45:32.437184 windmill_api-1.96.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-08 17:45:32.425184 windmill_api-1.96.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-08 17:45:32.621184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-08 17:45:32.465184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-08 17:45:32.557184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-08 17:45:32.689184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-08 17:45:32.657184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-08 17:45:32.701184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-08 17:45:32.733184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-08 17:45:32.753184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-08 17:45:32.865184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-08 17:45:32.789184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-08 17:45:32.873185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-08 17:45:20.809150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-08 17:45:32.913185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-08 17:45:32.921185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-08 17:45:20.833150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-08 17:45:32.969185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-08 17:45:20.589150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 17:45:21.365152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-08 17:45:32.989185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-08 17:45:33.129185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-08 17:45:33.041185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-08 17:45:33.089185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-08 17:45:33.133185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-08 17:45:33.173185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:20.849150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 17:45:33.177185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.725152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-08 17:45:33.213185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-08 17:45:33.221185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-08 17:45:33.337185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-08 17:45:33.285185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-08 17:45:33.325185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-08 17:45:33.377185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-08 17:45:33.385186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.705152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-08 17:45:33.445186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.433152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-08 17:45:33.433186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-08 17:45:33.473186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-08 17:45:33.501186 windmill_api-1.96.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-08 17:45:33.613186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-08 17:45:33.529186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 17:45:20.697150 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-08 17:45:33.565186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-08 17:45:33.625186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 17:45:33.733186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 17:45:20.829150 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 17:45:33.661186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 17:45:33.701186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 17:45:33.741186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 17:45:33.785186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 17:45:21.433152 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 17:45:33.781186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 17:45:33.841186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 17:45:21.321151 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 17:45:33.825186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 17:45:21.105151 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-08 17:45:33.865186 windmill_api-1.96.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-08 17:45:33.901186 windmill_api-1.96.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-08 17:45:33.921187 windmill_api-1.96.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-08 17:45:33.953187 windmill_api-1.96.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-08 17:45:33.953187 windmill_api-1.96.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-08 17:45:33.989187 windmill_api-1.96.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-08 17:45:34.017187 windmill_api-1.96.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-08 17:45:34.033187 windmill_api-1.96.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-08 17:45:34.061187 windmill_api-1.96.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-08 17:45:34.105187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-08 17:45:34.089187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-08 17:45:34.133187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-08 17:45:34.145187 windmill_api-1.96.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-08 17:45:34.161187 windmill_api-1.96.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-08 17:45:34.281187 windmill_api-1.96.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 17:45:34.197187 windmill_api-1.96.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-08 17:45:34.269187 windmill_api-1.96.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-08 17:45:34.297187 windmill_api-1.96.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-08 17:45:34.409187 windmill_api-1.96.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-08 17:45:34.349187 windmill_api-1.96.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-08 17:45:34.393187 windmill_api-1.96.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-08 17:45:34.437188 windmill_api-1.96.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-08 17:45:34.453188 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-08 17:45:21.469152 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-08 17:45:34.477187 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-08 17:45:21.013151 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-08 17:45:34.501188 windmill_api-1.96.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-08 17:45:34.541188 windmill_api-1.96.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-08 17:45:34.561188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.589188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.609188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.441151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.633188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-08 17:45:21.157151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-08 17:45:34.661188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.689188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.705188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:22.073154 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.737188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.821153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-08 17:45:20.957151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-08 17:45:34.749188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.789188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.837188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.885153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.833188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.873153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-08 17:45:20.945150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-08 17:45:34.913188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-08 17:45:34.881188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 17:45:21.253151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-08 17:45:34.929188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-08 17:45:35.029188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 17:45:34.985188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 17:45:35.029188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 17:45:35.101189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 17:45:35.073189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:22.085154 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 17:45:35.113189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:20.577150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 17:45:35.149189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 17:45:35.161189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-08 17:45:21.173151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-08 17:45:35.205189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-08 17:45:35.225189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 17:45:35.325189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 17:45:35.281189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 17:45:35.321189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 17:45:35.405189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 17:45:35.369189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.201151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 17:45:35.413189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:20.997151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 17:45:35.449189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 17:45:35.457189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-08 17:45:35.569190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 17:45:35.517189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 17:45:35.557190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 17:45:35.633190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 17:45:35.609190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:20.677150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 17:45:35.653190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 17:45:20.821150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 17:45:35.677190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 17:45:35.697190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:20.685150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-08 17:45:35.737190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-08 17:45:35.749190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 17:45:35.861190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 17:45:35.805190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 17:45:35.849190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 17:45:35.893190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 17:45:35.905190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:20.905151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 17:45:35.973190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.361151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 17:45:35.949190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 17:45:35.993190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:21.645152 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-08 17:45:36.013190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-08 17:45:21.905153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-08 17:45:36.037190 windmill_api-1.96.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-08 17:45:36.045190 windmill_api-1.96.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-08 17:45:36.097190 windmill_api-1.96.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-08 17:45:36.161191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-08 17:45:36.257191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-08 17:45:36.205191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-08 17:45:36.257191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-08 17:45:36.301191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:21.465152 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-08 17:45:36.293191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:20.749150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-08 17:45:36.333191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-08 17:45:36.353191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-08 17:45:36.449191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-08 17:45:36.413191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-08 17:45:36.457191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-08 17:45:36.497191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-08 17:45:36.541191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 17:45:20.877150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-08 17:45:36.537191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 17:45:20.765150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-08 17:45:36.581191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-08 17:45:36.589192 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-08 17:45:36.609192 windmill_api-1.96.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-08 17:45:36.657192 windmill_api-1.96.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-08 17:45:36.729192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-08 17:45:36.693192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-08 17:45:36.733192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-08 17:45:20.837150 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-08 17:45:36.769192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-08 17:45:36.813192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-08 17:45:36.905192 windmill_api-1.96.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-08 17:45:36.853192 windmill_api-1.96.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-08 17:45:36.897192 windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-08 17:45:21.825153 windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-08 17:45:36.949192 windmill_api-1.96.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-08 17:45:36.961192 windmill_api-1.96.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-08 17:45:21.861153 windmill_api-1.96.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-08 17:45:37.073192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-08 17:45:36.997192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-08 17:45:37.101192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-08 17:45:21.341151 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-08 17:45:37.113192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-08 17:45:37.153192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-08 17:45:21.129151 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-08 17:45:37.165192 windmill_api-1.96.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-08 17:45:37.213193 windmill_api-1.96.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-08 17:45:37.277193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-08 17:45:37.269193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 17:45:37.313193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 17:45:37.365193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 17:45:37.357193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 17:45:37.397193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 17:45:21.697152 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 17:45:37.413193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 17:45:37.437193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 17:45:37.529193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 17:45:37.493193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 17:45:37.533193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 17:45:37.585193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 17:45:37.573193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 17:45:21.125151 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 17:45:37.653193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 17:45:21.405151 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 17:45:37.625193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 17:45:37.669193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-08 17:45:37.697193 windmill_api-1.96.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-08 17:45:37.697193 windmill_api-1.96.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-08 17:45:37.729194 windmill_api-1.96.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-08 17:45:37.769194 windmill_api-1.96.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-08 17:45:37.769194 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-08 17:45:21.645152 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-08 17:45:37.809194 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-08 17:45:21.469152 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-08 17:45:37.929194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-08 17:45:37.865194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 17:45:37.905194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 17:45:37.953194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 17:45:37.969194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 17:45:20.625150 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 17:45:37.989194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 17:45:21.997153 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 17:45:38.017194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 17:45:38.029194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-08 17:45:20.881150 windmill_api-1.96.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-08 17:45:38.093194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:22.029153 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-08 17:45:38.061194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-08 17:45:38.129194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-08 17:45:21.165151 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-08 17:45:38.137194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-08 17:45:38.189194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-08 17:45:38.225195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-08 17:45:21.809153 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-08 17:45:38.221194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-08 17:45:38.293195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-08 17:45:21.209151 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-08 17:45:38.261195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-08 17:45:38.293195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-08 17:45:38.361195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-08 17:45:21.265151 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-08 17:45:38.329195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-08 17:45:38.401195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-08 17:45:21.705152 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-08 17:45:38.397195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-08 17:45:38.425195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-08 17:45:38.509195 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-08 17:45:21.485152 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-08 17:45:21.889153 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-08 17:45:38.465195 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-08 17:45:38.661195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-08 17:45:38.545195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-08 17:45:38.609195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-08 17:45:38.729195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-08 17:45:38.729195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-08 17:45:38.769195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-08 17:45:20.961151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 17:45:38.769195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-08 17:45:38.813196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-08 17:45:38.885196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-08 17:45:38.845196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 17:45:38.893196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 17:45:21.317151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 17:45:38.929196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 17:45:38.941196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 17:45:20.961151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-08 17:45:38.985196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-08 17:45:20.989151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 17:45:21.229151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-08 17:45:39.013196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-08 17:45:39.145196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-08 17:45:39.073196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-08 17:45:39.117196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-08 17:45:39.165196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-08 17:45:39.189196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-08 17:45:20.997151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-08 17:45:39.217196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-08 17:45:21.921153 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-08 17:45:39.229196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-08 17:45:39.301196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-08 17:45:39.345197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-08 17:45:39.365197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 17:45:39.393197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 17:45:39.417197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 17:45:39.433197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.445152 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 17:45:39.461197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.265151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 17:45:39.477197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 17:45:39.505197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-08 17:45:39.625197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-08 17:45:39.533197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-08 17:45:39.565197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-08 17:45:39.625197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-08 17:45:39.741197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-08 17:45:39.681197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 17:45:39.725197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 17:45:39.777197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 17:45:39.785197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 17:45:20.553150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 17:45:39.821198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 17:45:20.649150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 17:45:39.873198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 17:45:39.861198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-08 17:45:39.981198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-08 17:45:39.933198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-08 17:45:39.973198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-08 17:45:40.017198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-08 17:45:40.021198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 17:45:20.569150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-08 17:45:40.061198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-08 17:45:40.065198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-08 17:45:40.105198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-08 17:45:40.177198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-08 17:45:40.225198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-08 17:45:40.209198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-08 17:45:40.241198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-08 17:45:40.285198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-08 17:45:40.365198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-08 17:45:40.341199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-08 17:45:40.381199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-08 17:45:40.409199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-08 17:45:40.457199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-08 17:45:20.869150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-08 17:45:40.449199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-08 17:45:21.021151 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-08 17:45:40.485199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-08 17:45:40.493199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-08 17:45:40.597199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-08 17:45:40.545199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-08 17:45:40.589199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-08 17:45:40.637199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-08 17:45:40.637199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-08 17:45:20.805150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-08 17:45:40.709199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-08 17:45:22.065154 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-08 17:45:40.677199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-08 17:45:40.721199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-08 17:45:40.757199 windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-08 17:45:40.745199 windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-08 17:45:40.789199 windmill_api-1.96.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-08 17:45:40.785199 windmill_api-1.96.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-08 17:45:40.829199 windmill_api-1.96.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      325 2023-05-08 17:45:20.885151 windmill_api-1.96.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-08 17:45:40.817199 windmill_api-1.96.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-08 17:45:40.881199 windmill_api-1.96.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-08 17:45:40.853199 windmill_api-1.96.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-08 17:45:40.889200 windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-08 17:45:40.913200 windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-08 17:45:40.925200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-08 17:45:41.005200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-08 17:45:40.957200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-08 17:45:41.013200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-08 17:45:41.117200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-08 17:45:41.073200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-08 17:45:41.117200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-08 17:45:41.157200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-08 17:45:41.153200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.697152 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-08 17:45:41.197200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:20.957151 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-08 17:45:41.197200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-08 17:45:41.237200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-08 17:45:41.357200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-08 17:45:41.297200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-08 17:45:41.341200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-08 17:45:41.389201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-08 17:45:41.401200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-08 17:45:22.125154 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-08 17:45:41.433200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 17:45:41.445201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-08 17:45:41.521201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-08 17:45:41.497201 windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-08 17:45:22.041154 windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-08 17:45:41.553201 windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-08 17:45:41.553201 windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-08 17:45:21.117151 windmill_api-1.96.0/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-08 17:45:41.597201 windmill_api-1.96.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-08 17:45:41.609201 windmill_api-1.96.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-08 17:45:41.637201 windmill_api-1.96.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-08 17:45:41.677201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-08 17:45:41.661201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-08 17:45:41.725201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-08 17:45:21.221151 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-08 17:45:41.713201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-08 17:45:41.741201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-08 17:45:41.833201 windmill_api-1.96.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.765201 windmill_api-1.96.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-08 17:45:41.817201 windmill_api-1.96.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-08 17:45:41.857201 windmill_api-1.96.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-08 17:45:41.913201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:41.889201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.917201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-08 17:45:42.029202 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 17:45:41.945201 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 17:45:22.117154 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 17:45:21.357151 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.973202 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-08 17:45:42.141202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 17:45:42.057202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 17:45:21.641152 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 17:45:21.377151 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 17:45:42.093202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-08 17:45:42.197202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-08 17:45:42.241202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-08 17:45:21.049151 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-08 17:45:22.081154 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-08 17:45:42.229202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-08 17:45:20.757150 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-08 17:45:22.061154 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-08 17:45:42.265202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-08 17:45:42.281202 windmill_api-1.96.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-08 17:45:42.385202 windmill_api-1.96.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-08 17:45:42.321202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-08 17:45:42.357202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-08 17:45:42.397202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-08 17:45:20.661150 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-08 17:45:42.501202 windmill_api-1.96.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 17:45:42.425202 windmill_api-1.96.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-08 17:45:42.485202 windmill_api-1.96.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-08 17:45:42.521203 windmill_api-1.96.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-08 17:45:42.557203 windmill_api-1.96.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-08 17:45:20.809150 windmill_api-1.96.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-08 17:45:42.657203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-08 17:45:42.649203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-08 17:45:21.329151 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-08 17:45:42.689203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-08 17:45:42.693203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-08 17:45:42.733203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-08 17:45:42.749203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-08 17:45:20.597150 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-08 17:45:42.769203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-08 17:45:42.801203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-08 17:45:20.849150 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 17:45:42.809203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:21.193151 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-08 17:45:42.857203 windmill_api-1.96.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-08 17:45:42.833203 windmill_api-1.96.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-08 17:45:42.869203 windmill_api-1.96.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-08 17:45:21.013151 windmill_api-1.96.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 17:45:42.913203 windmill_api-1.96.0/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-08 17:45:42.957203 windmill_api-1.96.0/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-08 17:45:42.953203 windmill_api-1.96.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-08 17:45:42.997203 windmill_api-1.96.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:21.893153 windmill_api-1.96.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 17:45:43.001203 windmill_api-1.96.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-08 17:45:43.033203 windmill_api-1.96.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-08 17:45:21.249151 windmill_api-1.96.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-08 17:45:43.053204 windmill_api-1.96.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-08 17:45:21.937153 windmill_api-1.96.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-08 17:45:43.105204 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:20.773150 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-08 17:45:43.085204 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-08 17:45:43.161204 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-08 17:45:22.041154 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-08 17:45:21.413152 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-08 17:45:43.145204 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-08 17:45:43.341204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-08 17:45:43.189204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-08 17:45:43.289204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-08 17:45:43.405204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-08 17:45:43.381204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-08 17:45:43.421204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-08 17:45:20.941151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-08 17:45:43.445204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-08 17:45:43.533204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-08 17:45:21.229151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-08 17:45:43.565204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-08 17:45:43.569205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-08 17:45:43.605205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-08 17:45:21.081151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-08 17:45:43.609205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-08 17:45:43.657205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-08 17:45:21.337151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-08 17:45:43.661205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-08 17:45:21.893153 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:21.333151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-08 17:45:43.725205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-08 17:45:43.853205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-08 17:45:43.785205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-08 17:45:43.825205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-08 17:45:43.873205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-08 17:45:43.893205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-08 17:45:20.537150 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-08 17:45:43.917205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-08 17:45:21.517152 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 17:45:43.937205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-08 17:45:43.961205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-08 17:45:44.061205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-08 17:45:44.021206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-08 17:45:44.065205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-08 17:45:44.109206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-08 17:45:44.181206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-08 17:45:20.569150 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-08 17:45:44.153206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-08 17:45:21.025151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-08 17:45:44.193206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-08 17:45:44.229206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-08 17:45:44.237206 windmill_api-1.96.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-08 17:45:44.269206 windmill_api-1.96.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-08 17:45:44.281206 windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 17:45:44.301206 windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-08 17:45:44.429206 windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-08 17:45:44.333206 windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-08 17:45:44.385206 windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-08 17:45:44.437206 windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 17:45:44.477206 windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-08 17:45:44.493206 windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 17:45:44.525206 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-08 17:45:44.557206 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-08 17:45:21.589152 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-08 17:45:44.581206 windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-08 17:45:44.585206 windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-08 17:45:21.377151 windmill_api-1.96.0/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 17:45:44.629207 windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-08 17:45:20.541150 windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-08 17:45:44.633206 windmill_api-1.96.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-08 17:45:44.933207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-08 17:45:44.669207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-08 17:45:44.733207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-08 17:45:44.861207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-08 17:45:44.897207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 17:45:45.005207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 17:45:22.133154 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 17:45:44.973207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 17:45:45.029207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 17:45:21.537152 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-08 17:45:45.125208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-08 17:45:45.065207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-08 17:45:45.105208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-08 17:45:21.869153 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-08 17:45:45.145208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-08 17:45:45.173208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-08 17:45:45.193208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-08 17:45:22.145154 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-08 17:45:21.369151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-08 17:45:45.237208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-08 17:45:45.381208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-08 17:45:45.297208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 17:45:45.341208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 17:45:45.389208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 17:45:45.421208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.673152 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 17:45:45.429208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.149151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 17:45:45.465208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 17:45:45.469208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-08 17:45:45.585208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-08 17:45:45.601208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 17:45:45.621209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 17:45:45.649208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 17:45:45.673209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 17:45:21.373151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 17:45:45.693209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 17:45:20.969151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 17:45:45.713209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 17:45:45.737209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3045 2023-05-08 17:45:45.777209 windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item.py
--rw-r--r--   0        0        0     1294 2023-05-08 17:45:45.761209 windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     4884 2023-05-08 17:45:45.865209 windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 17:45:45.801209 windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-08 17:45:45.853209 windmill_api-1.96.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-08 17:45:46.029209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-08 17:45:45.897209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-08 17:45:45.925209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-08 17:45:46.057210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 17:45:46.061210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 17:45:21.793153 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 17:45:21.785153 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-08 17:45:46.153210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-08 17:45:46.125210 windmill_api-1.96.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-08 17:45:46.169210 windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-08 17:45:46.193210 windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-08 17:45:46.225210 windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-08 17:45:21.817153 windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-08 17:45:46.285210 windmill_api-1.96.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-08 17:45:46.261210 windmill_api-1.96.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-08 17:45:46.357210 windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 17:45:46.317210 windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-08 17:45:46.369210 windmill_api-1.96.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 17:45:46.401210 windmill_api-1.96.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-08 17:45:46.417210 windmill_api-1.96.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-08 17:45:46.449211 windmill_api-1.96.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-08 17:45:46.485211 windmill_api-1.96.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-08 17:45:21.509152 windmill_api-1.96.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-08 17:45:46.481211 windmill_api-1.96.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     2913 2023-05-08 17:45:46.537211 windmill_api-1.96.0/windmill_api/models/listable_raw_app.py
--rw-r--r--   0        0        0     1225 2023-05-08 17:45:46.513211 windmill_api-1.96.0/windmill_api/models/listable_raw_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-08 17:45:46.605211 windmill_api-1.96.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:46.565211 windmill_api-1.96.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-08 17:45:46.749211 windmill_api-1.96.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:46.633211 windmill_api-1.96.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-08 17:45:46.737211 windmill_api-1.96.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-08 17:45:46.777211 windmill_api-1.96.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-08 17:45:46.797211 windmill_api-1.96.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-08 17:45:46.837211 windmill_api-1.96.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-08 17:45:46.893211 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-08 17:45:21.545152 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-08 17:45:46.881212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-08 17:45:46.917212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-08 17:45:46.933212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-08 17:45:46.985212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-08 17:45:20.725150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 17:45:46.969212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-08 17:45:47.025212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-08 17:45:20.777150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-08 17:45:47.021212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 17:45:20.729150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-08 17:45:47.081212 windmill_api-1.96.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-08 17:45:47.057212 windmill_api-1.96.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-08 17:45:47.165212 windmill_api-1.96.0/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-08 17:45:21.593152 windmill_api-1.96.0/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.829153 windmill_api-1.96.0/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-08 17:45:47.117212 windmill_api-1.96.0/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-08 17:45:47.241212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-08 17:45:47.345213 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-08 17:45:21.033151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-08 17:45:21.153151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-08 17:45:47.277212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-08 17:45:20.621150 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-08 17:45:21.145151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-08 17:45:47.313212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-08 17:45:47.369213 windmill_api-1.96.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-08 17:45:47.401213 windmill_api-1.96.0/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-08 17:45:47.413213 windmill_api-1.96.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-08 17:45:47.465213 windmill_api-1.96.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 17:45:47.441213 windmill_api-1.96.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-08 17:45:47.585213 windmill_api-1.96.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-08 17:45:47.581213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-08 17:45:47.641213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-08 17:45:47.629213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-08 17:45:47.677214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-08 17:45:47.681213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-08 17:45:20.993151 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-08 17:45:47.717213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-08 17:45:21.917153 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-08 17:45:47.725214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-08 17:45:47.757214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-08 17:45:47.841214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-08 17:45:47.813214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-08 17:45:47.917214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-08 17:45:47.893214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-08 17:45:47.933214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 17:45:21.625152 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-08 17:45:47.957214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 17:45:20.753150 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-08 17:45:47.981214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-08 17:45:47.997214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-08 17:45:48.041214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-08 17:45:48.025214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-08 17:45:48.085214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-08 17:45:48.257215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-08 17:45:48.145215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-08 17:45:48.185215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-08 17:45:48.233215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-08 17:45:48.277215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-08 17:45:20.877150 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-08 17:45:48.313215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 17:45:20.825150 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-08 17:45:48.321215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-08 17:45:48.365215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-08 17:45:48.513215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-08 17:45:48.429215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-08 17:45:48.473215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-08 17:45:48.521216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-08 17:45:48.557216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-08 17:45:48.573216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:22.069154 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-08 17:45:48.601216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-08 17:45:48.621216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-08 17:45:48.645216 windmill_api-1.96.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-08 17:45:48.673216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-08 17:45:48.689216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 17:45:20.929150 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-08 17:45:48.717216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 17:45:20.721150 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-08 17:45:21.009151 windmill_api-1.96.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-08 17:45:48.749216 windmill_api-1.96.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-08 17:45:48.861216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-08 17:45:48.793216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 17:45:21.953153 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 17:45:48.833216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 17:45:21.389151 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-08 17:45:21.429152 windmill_api-1.96.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-08 17:45:48.905216 windmill_api-1.96.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-08 17:45:22.089154 windmill_api-1.96.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-08 17:45:48.897216 windmill_api-1.96.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-08 17:45:48.929216 windmill_api-1.96.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-08 17:45:48.961217 windmill_api-1.96.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-08 17:45:48.961217 windmill_api-1.96.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-08 17:45:21.857153 windmill_api-1.96.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-08 17:45:49.005217 windmill_api-1.96.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-08 17:45:49.021217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-08 17:45:49.093217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-08 17:45:20.733150 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-08 17:45:49.065217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-08 17:45:49.101217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-08 17:45:49.133217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-08 17:45:49.157217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-08 17:45:21.741152 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-08 17:45:49.169217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-08 17:45:49.209217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-08 17:45:20.561150 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-08 17:45:49.205217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-08 17:45:21.981153 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-08 17:45:49.485218 windmill_api-1.96.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-08 17:45:49.237217 windmill_api-1.96.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-08 17:45:49.301217 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-08 17:45:49.429218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-08 17:45:49.557218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 17:45:49.529218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-08 17:45:21.429152 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-08 17:45:49.565218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-08 17:45:49.613218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-08 17:45:49.685218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-08 17:45:49.657218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 17:45:49.701218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-08 17:45:20.845150 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-08 17:45:49.725218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-08 17:45:49.765219 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-08 17:45:20.549150 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-08 17:45:49.869219 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-08 17:45:21.829153 windmill_api-1.96.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.049151 windmill_api-1.96.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-08 17:45:49.829219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-08 17:45:49.945219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-08 17:45:49.925219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-08 17:45:49.969219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-08 17:45:49.989219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-08 17:45:50.009219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:21.605152 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 17:45:50.037219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 17:45:21.517152 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 17:45:50.053219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-08 17:45:50.085219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-08 17:45:50.165219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-08 17:45:50.141219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-08 17:45:50.285220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-08 17:45:50.213220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-08 17:45:50.269220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 17:45:21.817153 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-08 17:45:50.317220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 17:45:21.353151 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-08 17:45:50.329220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-08 17:45:50.357220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-08 17:45:50.397220 windmill_api-1.96.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-08 17:45:50.409220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-08 17:45:50.437220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-08 17:45:50.537220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-08 17:45:21.297151 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-08 17:45:21.973153 windmill_api-1.96.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-08 17:45:50.477220 windmill_api-1.96.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-08 17:45:50.517220 windmill_api-1.96.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      328 2023-05-08 17:45:21.113151 windmill_api-1.96.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-08 17:45:50.561221 windmill_api-1.96.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-08 17:45:50.577221 windmill_api-1.96.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-08 17:45:50.633221 windmill_api-1.96.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-08 17:45:50.605221 windmill_api-1.96.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-08 17:45:50.653221 windmill_api-1.96.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-08 17:45:50.661221 windmill_api-1.96.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 17:45:50.681221 windmill_api-1.96.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-08 17:45:50.725221 windmill_api-1.96.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-08 17:45:50.729221 windmill_api-1.96.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-08 17:45:50.773221 windmill_api-1.96.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-08 17:45:50.757221 windmill_api-1.96.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-08 17:45:50.801221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-08 17:45:50.797221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 17:45:50.857221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-08 17:45:50.913221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-08 17:45:50.913221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-08 17:45:50.957221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-08 17:45:50.965222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-08 17:45:51.001222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 17:45:20.789150 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 17:45:51.005221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 17:45:20.713150 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-08 17:45:51.061222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-08 17:45:51.049222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-08 17:45:51.241222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-08 17:45:51.125222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-08 17:45:51.169222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-08 17:45:51.321222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-08 17:45:51.285222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 17:45:21.901153 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-08 17:45:51.333222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 17:45:21.657152 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-08 17:45:51.361222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-08 17:45:51.377222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-08 17:45:51.389222 windmill_api-1.96.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-08 17:45:51.405223 windmill_api-1.96.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-08 17:45:51.445223 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-08 17:45:51.433223 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-08 17:45:21.785153 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-08 17:45:51.465223 windmill_api-1.96.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-08 17:45:51.473223 windmill_api-1.96.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-08 17:45:21.721152 windmill_api-1.96.0/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-08 17:45:51.553223 windmill_api-1.96.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-08 17:45:51.505223 windmill_api-1.96.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-08 17:45:51.533223 windmill_api-1.96.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-08 17:45:51.669223 windmill_api-1.96.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-08 17:45:51.581223 windmill_api-1.96.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-08 17:45:51.609223 windmill_api-1.96.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-08 17:45:21.605152 windmill_api-1.96.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-08 17:45:21.909153 windmill_api-1.96.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-08 17:45:51.645223 windmill_api-1.96.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-08 17:45:51.677223 windmill_api-1.96.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-08 17:45:51.697223 windmill_api-1.96.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-08 17:45:51.721223 windmill_api-1.96.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-08 17:45:51.741223 windmill_api-1.96.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-08 17:45:51.769223 windmill_api-1.96.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      209 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-08 17:45:51.785223 windmill_api-1.96.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-08 17:45:21.481152 windmill_api-1.96.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-08 17:45:51.825224 windmill_api-1.96.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-08 17:45:51.849223 windmill_api-1.96.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-08 17:45:51.873224 windmill_api-1.96.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      211 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-08 17:45:51.909224 windmill_api-1.96.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 17:45:52.033224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 17:45:51.945224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 17:45:51.977224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-08 17:45:52.153224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-08 17:45:52.069224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-08 17:45:52.129224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-08 17:45:52.245225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-08 17:45:52.213225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-08 17:45:52.257225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-08 17:45:52.293225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-08 17:45:52.305225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 17:45:21.765153 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-08 17:45:52.333225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-08 17:45:52.345225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-08 17:45:52.377225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-08 17:45:52.469225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-08 17:45:52.437225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-08 17:45:52.477225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-08 17:45:52.521225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-08 17:45:52.517225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-08 17:45:21.349151 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-08 17:45:52.557225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-08 17:45:21.613152 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-08 17:45:52.561225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-08 17:45:52.597226 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-08 17:45:52.605225 windmill_api-1.96.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-08 17:45:52.737226 windmill_api-1.96.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-08 17:45:52.649226 windmill_api-1.96.0/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-08 17:45:52.789226 windmill_api-1.96.0/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     1985 2023-05-08 17:45:52.785226 windmill_api-1.96.0/windmill_api/models/update_raw_app_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-08 17:45:52.837226 windmill_api-1.96.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-08 17:45:52.833226 windmill_api-1.96.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-08 17:45:52.869226 windmill_api-1.96.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-08 17:45:52.881226 windmill_api-1.96.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 17:45:52.905226 windmill_api-1.96.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-08 17:45:52.929226 windmill_api-1.96.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-08 17:45:52.957226 windmill_api-1.96.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-08 17:45:52.969226 windmill_api-1.96.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-08 17:45:53.045226 windmill_api-1.96.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-08 17:45:53.001226 windmill_api-1.96.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-08 17:45:53.045226 windmill_api-1.96.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-08 17:45:53.085227 windmill_api-1.96.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-08 17:45:53.137227 windmill_api-1.96.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-08 17:45:53.121227 windmill_api-1.96.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-08 17:45:53.209227 windmill_api-1.96.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-08 17:45:53.177227 windmill_api-1.96.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-08 17:45:53.233227 windmill_api-1.96.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-08 17:45:53.257227 windmill_api-1.96.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-08 17:45:53.277227 windmill_api-1.96.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-08 17:45:08.361165 windmill_api-1.96.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-08 17:45:53.281227 windmill_api-1.96.0/windmill_api/types.py
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-08 19:21:20.939801 windmill_api-1.96.1/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-08 19:21:20.943801 windmill_api-1.96.1/README.md
+-rw-r--r--   0        0        0      717 2023-05-08 19:21:20.939801 windmill_api-1.96.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-08 19:20:47.203207 windmill_api-1.96.1/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-08 19:20:47.699214 windmill_api-1.96.1/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.831216 windmill_api-1.96.1/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-08 19:20:58.411395 windmill_api-1.96.1/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-08 19:20:58.415395 windmill_api-1.96.1/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-08 19:20:58.443395 windmill_api-1.96.1/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-08 19:20:58.479396 windmill_api-1.96.1/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-08 19:20:58.483396 windmill_api-1.96.1/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-08 19:20:58.531397 windmill_api-1.96.1/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-08 19:20:58.523397 windmill_api-1.96.1/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-08 19:20:58.579398 windmill_api-1.96.1/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-08 19:20:58.587398 windmill_api-1.96.1/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-08 19:20:58.607398 windmill_api-1.96.1/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-08 19:20:58.675399 windmill_api-1.96.1/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-08 19:20:58.643399 windmill_api-1.96.1/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-08 19:20:58.679400 windmill_api-1.96.1/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.739215 windmill_api-1.96.1/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-08 19:20:58.715400 windmill_api-1.96.1/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-08 19:20:58.787402 windmill_api-1.96.1/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-08 19:20:58.747401 windmill_api-1.96.1/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-08 19:20:58.775401 windmill_api-1.96.1/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-08 19:20:58.807402 windmill_api-1.96.1/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-08 19:20:58.815402 windmill_api-1.96.1/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-08 19:20:58.843403 windmill_api-1.96.1/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-08 19:20:58.847403 windmill_api-1.96.1/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.799216 windmill_api-1.96.1/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-08 19:20:58.879403 windmill_api-1.96.1/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-08 19:20:58.875403 windmill_api-1.96.1/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-08 19:20:58.931404 windmill_api-1.96.1/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-08 19:20:58.919404 windmill_api-1.96.1/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-08 19:20:58.987405 windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-08 19:20:58.971405 windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-08 19:20:59.031406 windmill_api-1.96.1/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-08 19:20:59.023406 windmill_api-1.96.1/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-08 19:20:59.055407 windmill_api-1.96.1/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-08 19:20:59.123408 windmill_api-1.96.1/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-08 19:20:59.091407 windmill_api-1.96.1/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-08 19:20:59.123408 windmill_api-1.96.1/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.883217 windmill_api-1.96.1/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-08 19:20:59.159408 windmill_api-1.96.1/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-08 19:20:59.151408 windmill_api-1.96.1/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-08 19:20:59.179409 windmill_api-1.96.1/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-08 19:20:59.203409 windmill_api-1.96.1/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-08 19:20:59.219410 windmill_api-1.96.1/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-08 19:20:59.255410 windmill_api-1.96.1/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-08 19:20:59.303411 windmill_api-1.96.1/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-08 19:20:59.287411 windmill_api-1.96.1/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-08 19:20:59.355412 windmill_api-1.96.1/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.887217 windmill_api-1.96.1/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-08 19:20:59.335412 windmill_api-1.96.1/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-08 19:20:59.375413 windmill_api-1.96.1/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-08 19:20:59.391413 windmill_api-1.96.1/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.875217 windmill_api-1.96.1/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-08 19:20:59.407413 windmill_api-1.96.1/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-08 19:20:59.423413 windmill_api-1.96.1/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-08 19:20:59.435414 windmill_api-1.96.1/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-08 19:20:59.467414 windmill_api-1.96.1/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-08 19:20:59.483415 windmill_api-1.96.1/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-08 19:20:59.543416 windmill_api-1.96.1/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-08 19:20:59.511415 windmill_api-1.96.1/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-08 19:20:59.559416 windmill_api-1.96.1/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-08 19:20:59.595417 windmill_api-1.96.1/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-08 19:20:59.587417 windmill_api-1.96.1/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-08 19:20:59.683418 windmill_api-1.96.1/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-08 19:20:59.667418 windmill_api-1.96.1/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-08 19:20:59.699418 windmill_api-1.96.1/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-08 19:20:59.715419 windmill_api-1.96.1/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-08 19:20:59.779420 windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 19:20:59.759420 windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-08 19:20:59.799420 windmill_api-1.96.1/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-08 19:20:59.819421 windmill_api-1.96.1/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-08 19:20:59.831421 windmill_api-1.96.1/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-08 19:20:59.859421 windmill_api-1.96.1/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:20:59.863422 windmill_api-1.96.1/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-08 19:20:59.903422 windmill_api-1.96.1/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-08 19:20:59.919422 windmill_api-1.96.1/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-08 19:20:59.959423 windmill_api-1.96.1/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-08 19:20:59.975424 windmill_api-1.96.1/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-08 19:21:00.147427 windmill_api-1.96.1/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-08 19:21:00.147427 windmill_api-1.96.1/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-08 19:21:00.295430 windmill_api-1.96.1/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-08 19:21:00.179427 windmill_api-1.96.1/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-08 19:21:00.211428 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-08 19:21:00.255429 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 19:21:00.303430 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-08 19:21:00.351431 windmill_api-1.96.1/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-08 19:21:00.343430 windmill_api-1.96.1/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-08 19:21:00.403432 windmill_api-1.96.1/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-08 19:21:00.447432 windmill_api-1.96.1/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-08 19:21:00.447432 windmill_api-1.96.1/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-08 19:21:00.491433 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-08 19:21:00.491433 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-08 19:21:00.567435 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.771215 windmill_api-1.96.1/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-08 19:21:00.535434 windmill_api-1.96.1/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-08 19:21:00.563434 windmill_api-1.96.1/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-08 19:21:00.591435 windmill_api-1.96.1/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-08 19:21:00.611435 windmill_api-1.96.1/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-08 19:21:00.619435 windmill_api-1.96.1/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-08 19:21:00.639436 windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-08 19:21:00.655436 windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-08 19:21:00.671436 windmill_api-1.96.1/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.867217 windmill_api-1.96.1/windmill_api/api/raw_app/__init__.py
+-rw-r--r--   0        0        0     2033 2023-05-08 19:21:00.683437 windmill_api-1.96.1/windmill_api/api/raw_app/create_raw_app.py
+-rw-r--r--   0        0        0     1781 2023-05-08 19:21:00.703437 windmill_api-1.96.1/windmill_api/api/raw_app/delete_raw_app.py
+-rw-r--r--   0        0        0     2786 2023-05-08 19:21:00.723437 windmill_api-1.96.1/windmill_api/api/raw_app/exists_raw_app.py
+-rw-r--r--   0        0        0     1979 2023-05-08 19:21:00.735438 windmill_api-1.96.1/windmill_api/api/raw_app/get_raw_app_data.py
+-rw-r--r--   0        0        0     7349 2023-05-08 19:21:00.831439 windmill_api-1.96.1/windmill_api/api/raw_app/list_raw_apps.py
+-rw-r--r--   0        0        0     2166 2023-05-08 19:21:00.767438 windmill_api-1.96.1/windmill_api/api/raw_app/update_raw_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.775215 windmill_api-1.96.1/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 19:21:00.799439 windmill_api-1.96.1/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-08 19:21:00.831439 windmill_api-1.96.1/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:00.859440 windmill_api-1.96.1/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-08 19:21:00.859440 windmill_api-1.96.1/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-08 19:21:00.919441 windmill_api-1.96.1/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-08 19:21:00.903441 windmill_api-1.96.1/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-08 19:21:00.943441 windmill_api-1.96.1/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-08 19:21:00.959442 windmill_api-1.96.1/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-08 19:21:00.975442 windmill_api-1.96.1/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-08 19:21:01.027443 windmill_api-1.96.1/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-08 19:21:01.015443 windmill_api-1.96.1/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-08 19:21:01.059444 windmill_api-1.96.1/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-08 19:21:01.059444 windmill_api-1.96.1/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-08 19:21:01.123445 windmill_api-1.96.1/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-08 19:21:01.087444 windmill_api-1.96.1/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.871217 windmill_api-1.96.1/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 19:21:01.119445 windmill_api-1.96.1/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.147445 windmill_api-1.96.1/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-08 19:21:01.163446 windmill_api-1.96.1/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-08 19:21:01.187446 windmill_api-1.96.1/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-08 19:21:01.223447 windmill_api-1.96.1/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-08 19:21:01.227447 windmill_api-1.96.1/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-08 19:21:01.255447 windmill_api-1.96.1/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-08 19:21:01.283448 windmill_api-1.96.1/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.783215 windmill_api-1.96.1/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-08 19:21:01.299448 windmill_api-1.96.1/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-08 19:21:01.307448 windmill_api-1.96.1/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 19:21:01.343449 windmill_api-1.96.1/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-08 19:21:01.335449 windmill_api-1.96.1/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-08 19:21:01.375450 windmill_api-1.96.1/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-08 19:21:01.383450 windmill_api-1.96.1/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 19:21:01.415450 windmill_api-1.96.1/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-08 19:21:01.423450 windmill_api-1.96.1/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-08 19:21:01.451451 windmill_api-1.96.1/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-08 19:21:01.455451 windmill_api-1.96.1/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-08 19:21:01.491452 windmill_api-1.96.1/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-08 19:21:01.515452 windmill_api-1.96.1/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-08 19:21:01.531453 windmill_api-1.96.1/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-08 19:21:01.559453 windmill_api-1.96.1/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-08 19:21:01.571453 windmill_api-1.96.1/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-08 19:21:01.595454 windmill_api-1.96.1/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-08 19:21:01.615454 windmill_api-1.96.1/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-08 19:21:01.727456 windmill_api-1.96.1/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-08 19:21:01.655455 windmill_api-1.96.1/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.679455 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.707456 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-08 19:21:01.739456 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.715214 windmill_api-1.96.1/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-08 19:21:01.755457 windmill_api-1.96.1/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-08 19:21:01.763457 windmill_api-1.96.1/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.743215 windmill_api-1.96.1/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-08 19:21:01.787457 windmill_api-1.96.1/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-08 19:21:01.787457 windmill_api-1.96.1/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-08 19:21:01.835458 windmill_api-1.96.1/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-08 19:21:01.819458 windmill_api-1.96.1/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-08 19:21:01.843458 windmill_api-1.96.1/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-08 19:21:01.899459 windmill_api-1.96.1/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-08 19:21:01.871459 windmill_api-1.96.1/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-08 19:21:01.899459 windmill_api-1.96.1/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-08 19:21:01.923460 windmill_api-1.96.1/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-08 19:21:01.939460 windmill_api-1.96.1/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-08 19:21:01.951460 windmill_api-1.96.1/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-08 19:21:01.967460 windmill_api-1.96.1/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-08 19:21:01.987461 windmill_api-1.96.1/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-08 19:21:02.007461 windmill_api-1.96.1/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-08 19:21:02.015461 windmill_api-1.96.1/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-08 19:21:02.043462 windmill_api-1.96.1/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-08 19:21:02.055462 windmill_api-1.96.1/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-08 19:21:02.083463 windmill_api-1.96.1/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-08 19:21:02.111463 windmill_api-1.96.1/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-08 19:21:02.119463 windmill_api-1.96.1/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:02.143464 windmill_api-1.96.1/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-08 19:21:02.147464 windmill_api-1.96.1/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-08 19:21:02.167464 windmill_api-1.96.1/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-08 19:21:02.175464 windmill_api-1.96.1/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-08 19:21:02.199465 windmill_api-1.96.1/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-08 19:21:02.211465 windmill_api-1.96.1/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-08 19:21:02.267466 windmill_api-1.96.1/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.767215 windmill_api-1.96.1/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-08 19:21:02.247466 windmill_api-1.96.1/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-08 19:21:02.295467 windmill_api-1.96.1/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-08 19:21:02.307467 windmill_api-1.96.1/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-08 19:21:02.343467 windmill_api-1.96.1/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-08 19:21:02.351468 windmill_api-1.96.1/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-08 19:21:02.383468 windmill_api-1.96.1/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-08 19:21:02.391468 windmill_api-1.96.1/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-08 19:21:02.419469 windmill_api-1.96.1/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-08 19:21:02.447469 windmill_api-1.96.1/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:20:47.755215 windmill_api-1.96.1/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-08 19:21:02.451470 windmill_api-1.96.1/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-08 19:21:02.475470 windmill_api-1.96.1/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.479470 windmill_api-1.96.1/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-08 19:21:02.507470 windmill_api-1.96.1/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-08 19:21:02.503471 windmill_api-1.96.1/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-08 19:21:02.531471 windmill_api-1.96.1/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-08 19:21:02.539471 windmill_api-1.96.1/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-08 19:21:02.563471 windmill_api-1.96.1/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.567472 windmill_api-1.96.1/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.587472 windmill_api-1.96.1/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-08 19:21:02.607472 windmill_api-1.96.1/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-08 19:21:02.647473 windmill_api-1.96.1/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-08 19:21:02.663473 windmill_api-1.96.1/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-08 19:21:02.679474 windmill_api-1.96.1/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-08 19:21:02.707474 windmill_api-1.96.1/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-08 19:21:02.715474 windmill_api-1.96.1/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-08 19:21:02.743475 windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-08 19:21:02.767475 windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-08 19:21:02.771475 windmill_api-1.96.1/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-08 19:21:02.795476 windmill_api-1.96.1/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-08 19:21:20.935801 windmill_api-1.96.1/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-08 19:21:02.819476 windmill_api-1.96.1/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-08 19:21:02.847477 windmill_api-1.96.1/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      325 2023-05-08 19:20:56.991370 windmill_api-1.96.1/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-08 19:21:02.875477 windmill_api-1.96.1/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-08 19:21:02.903478 windmill_api-1.96.1/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-08 19:21:02.923478 windmill_api-1.96.1/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-08 19:21:02.955479 windmill_api-1.96.1/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-08 19:20:57.483378 windmill_api-1.96.1/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-08 19:21:02.987479 windmill_api-1.96.1/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-08 19:21:03.023480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-08 19:20:57.531379 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.019480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-08 19:21:03.039480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-08 19:21:03.079481 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-08 19:21:03.063481 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-08 19:21:03.111482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-08 19:20:57.095371 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-08 19:21:03.103482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-08 19:21:03.123482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-08 19:21:03.139482 windmill_api-1.96.1/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-08 19:21:03.215484 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-08 19:21:03.159483 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-08 19:20:57.767383 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-08 19:20:57.455378 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-08 19:21:03.187483 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-08 19:21:03.239484 windmill_api-1.96.1/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-08 19:20:57.523379 windmill_api-1.96.1/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-08 19:20:57.411377 windmill_api-1.96.1/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-08 19:21:03.239484 windmill_api-1.96.1/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-08 19:21:03.279485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 19:21:03.299485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 19:20:57.431377 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 19:21:03.307485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 19:21:03.359486 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 19:21:03.339486 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 19:21:03.403487 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 19:20:57.595380 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 19:21:03.387487 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 19:21:03.423488 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 19:20:57.535379 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 19:21:03.431488 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 19:21:03.459488 windmill_api-1.96.1/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-08 19:21:03.471488 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 19:21:03.539490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 19:21:03.511489 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 19:21:03.547490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 19:21:03.571490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 19:21:03.579490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.503378 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.599491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 19:21:03.611491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 19:21:03.627491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-08 19:21:03.651492 windmill_api-1.96.1/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-08 19:21:03.663492 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 19:21:03.735493 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 19:21:03.723493 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 19:21:03.751494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 19:21:03.799494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 19:21:03.779494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.419377 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.807494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:56.975369 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 19:21:03.831495 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 19:21:03.835495 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 19:21:03.915496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 19:21:03.875496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 19:21:03.903496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 19:21:03.935497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 19:21:03.947497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 19:21:03.963497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 19:20:57.679381 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 19:21:03.995498 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 19:21:03.991498 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 19:20:57.511379 windmill_api-1.96.1/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-08 19:21:04.015498 windmill_api-1.96.1/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 19:21:04.015498 windmill_api-1.96.1/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-08 19:21:04.151501 windmill_api-1.96.1/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-08 19:21:04.035499 windmill_api-1.96.1/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 19:21:04.103500 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-08 19:21:04.187502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-08 19:21:04.219502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-08 19:21:04.215502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-08 19:20:57.691382 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-08 19:21:04.239503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-08 19:21:04.259503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-08 19:20:56.955369 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-08 19:21:04.323504 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-08 19:21:04.283503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 19:21:04.311504 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-08 19:20:56.719365 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-08 19:21:04.343505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-08 19:21:04.355505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-08 19:20:57.767383 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-08 19:21:04.383505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-08 19:20:57.187373 windmill_api-1.96.1/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-08 19:20:56.707365 windmill_api-1.96.1/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-08 19:21:04.403506 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-08 19:21:04.463507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-08 19:21:04.487507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 19:21:04.495507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 19:21:04.519508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 19:21:04.527508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.279374 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 19:21:04.547508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.275375 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 19:21:04.559508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 19:21:04.575509 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-08 19:21:04.675511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-08 19:21:04.615510 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-08 19:21:04.643510 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-08 19:21:04.675511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-08 19:21:04.707511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-08 19:20:57.079371 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-08 19:21:04.703511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-08 19:20:57.115372 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-08 19:21:04.731512 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-08 19:21:04.739512 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-08 19:21:04.755512 windmill_api-1.96.1/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-08 19:21:04.779513 windmill_api-1.96.1/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-08 19:21:04.783513 windmill_api-1.96.1/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-08 19:21:04.807513 windmill_api-1.96.1/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-08 19:21:04.811513 windmill_api-1.96.1/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-08 19:21:04.843514 windmill_api-1.96.1/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 19:21:04.875514 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:57.775383 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 19:21:04.871514 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 19:21:04.895515 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-08 19:21:04.903515 windmill_api-1.96.1/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-08 19:20:57.231374 windmill_api-1.96.1/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-08 19:21:04.923515 windmill_api-1.96.1/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-08 19:21:04.939515 windmill_api-1.96.1/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-08 19:21:04.951516 windmill_api-1.96.1/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-08 19:21:04.963516 windmill_api-1.96.1/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-08 19:21:04.975516 windmill_api-1.96.1/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-08 19:21:04.991516 windmill_api-1.96.1/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-08 19:21:05.003517 windmill_api-1.96.1/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-08 19:20:56.735365 windmill_api-1.96.1/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     1732 2023-05-08 19:21:05.019517 windmill_api-1.96.1/windmill_api/models/create_raw_app_json_body.py
+-rw-r--r--   0        0        0     2094 2023-05-08 19:21:05.071518 windmill_api-1.96.1/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-08 19:21:05.051518 windmill_api-1.96.1/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-08 19:21:05.083518 windmill_api-1.96.1/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-08 19:21:05.115519 windmill_api-1.96.1/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:05.103519 windmill_api-1.96.1/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-08 19:21:05.175520 windmill_api-1.96.1/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-08 19:20:57.771383 windmill_api-1.96.1/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-08 19:20:56.711365 windmill_api-1.96.1/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:05.139519 windmill_api-1.96.1/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-08 19:21:05.179520 windmill_api-1.96.1/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-08 19:21:05.239521 windmill_api-1.96.1/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-08 19:21:05.215521 windmill_api-1.96.1/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-08 19:21:05.243521 windmill_api-1.96.1/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-08 19:21:05.275522 windmill_api-1.96.1/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-08 19:21:05.287522 windmill_api-1.96.1/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-08 19:21:05.303522 windmill_api-1.96.1/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-08 19:21:05.315523 windmill_api-1.96.1/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-08 19:21:05.327523 windmill_api-1.96.1/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-08 19:21:05.491526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-08 19:21:05.347523 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-08 19:21:05.391524 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-08 19:21:05.475525 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-08 19:21:05.499526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-08 19:21:05.527526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-08 19:21:05.523526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-08 19:21:05.559527 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-08 19:21:05.611528 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-08 19:21:05.615528 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-08 19:21:05.647529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-08 19:20:56.875368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-08 19:21:05.643529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-08 19:21:05.679529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-08 19:20:56.895368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-08 19:21:05.687529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 19:20:57.247374 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-08 19:21:05.735530 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-08 19:21:05.771531 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-08 19:21:05.775531 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-08 19:21:05.803532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-08 19:21:05.807532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-08 19:21:05.883533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 19:21:05.839532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.495378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-08 19:21:05.867533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-08 19:21:05.895533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-08 19:21:05.971535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-08 19:21:05.935534 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-08 19:21:05.983535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-08 19:21:06.007535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-08 19:21:06.015535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.479378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-08 19:21:06.039536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.295375 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-08 19:21:06.043536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-08 19:21:06.075536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-08 19:21:06.071536 windmill_api-1.96.1/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-08 19:21:06.163538 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-08 19:21:06.095537 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 19:20:56.795366 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-08 19:21:06.123537 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-08 19:21:06.163538 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 19:21:06.231539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 19:20:56.891368 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 19:21:06.195539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 19:21:06.223539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 19:21:06.251540 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 19:21:06.319541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 19:21:06.275540 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 19:21:06.311541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 19:20:57.215373 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 19:21:06.335541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 19:20:57.071371 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-08 19:21:06.347541 windmill_api-1.96.1/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-08 19:21:06.403542 windmill_api-1.96.1/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-08 19:21:06.379542 windmill_api-1.96.1/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-08 19:21:06.411543 windmill_api-1.96.1/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-08 19:21:06.423543 windmill_api-1.96.1/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-08 19:21:06.435543 windmill_api-1.96.1/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-08 19:21:06.459543 windmill_api-1.96.1/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-08 19:21:06.467543 windmill_api-1.96.1/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-08 19:21:06.491544 windmill_api-1.96.1/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-08 19:21:06.515544 windmill_api-1.96.1/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-08 19:21:06.511544 windmill_api-1.96.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-08 19:21:06.543545 windmill_api-1.96.1/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-08 19:21:06.543545 windmill_api-1.96.1/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-08 19:21:06.563545 windmill_api-1.96.1/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-08 19:21:06.615546 windmill_api-1.96.1/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 19:21:06.583546 windmill_api-1.96.1/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-08 19:21:06.635547 windmill_api-1.96.1/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-08 19:21:06.639546 windmill_api-1.96.1/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-08 19:21:06.715548 windmill_api-1.96.1/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-08 19:21:06.679547 windmill_api-1.96.1/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-08 19:21:06.763549 windmill_api-1.96.1/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-08 19:21:06.787549 windmill_api-1.96.1/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-08 19:21:06.799549 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-08 19:20:57.319375 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-08 19:21:06.815550 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-08 19:20:57.015370 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-08 19:21:06.831550 windmill_api-1.96.1/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-08 19:21:06.843550 windmill_api-1.96.1/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-08 19:21:06.879551 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-08 19:21:06.879551 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 19:21:06.911552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.299375 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 19:21:06.915552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-08 19:20:57.103371 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-08 19:21:06.951552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-08 19:21:06.955552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 19:21:06.979553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.743383 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 19:21:06.991553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-08 19:20:56.979369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-08 19:21:07.011553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-08 19:21:07.031554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 19:21:07.043554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.611380 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 19:21:07.063554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.599380 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-08 19:20:56.971369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-08 19:21:07.099555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-08 19:21:07.091555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 19:20:57.167373 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-08 19:21:07.123555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-08 19:21:07.227557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 19:21:07.199557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 19:21:07.231557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 19:21:07.259558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 19:21:07.263558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:57.751383 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 19:21:07.287558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:56.707365 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 19:21:07.295558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 19:21:07.315559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-08 19:20:57.115372 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-08 19:21:07.339559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-08 19:21:07.351559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 19:21:07.427561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 19:21:07.391560 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 19:21:07.419561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 19:21:07.451561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 19:21:07.459561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.131372 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 19:21:07.483562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 19:21:07.487562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 19:21:07.511562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-08 19:21:07.615564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 19:21:07.599564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 19:21:07.631564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 19:21:07.647565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 19:21:07.659565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:56.779366 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 19:21:07.679565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 19:20:56.883368 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 19:21:07.687565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 19:21:07.711566 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:56.783366 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-08 19:21:07.727566 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-08 19:21:07.747567 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 19:21:07.811568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 19:21:07.787567 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 19:21:07.815568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 19:21:07.843568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 19:21:07.847568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:56.943369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 19:21:07.875569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.243374 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 19:21:07.875569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 19:21:07.903569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-08 19:21:07.907569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-08 19:20:57.623381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-08 19:21:07.991571 windmill_api-1.96.1/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-08 19:21:07.931570 windmill_api-1.96.1/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-08 19:21:08.015571 windmill_api-1.96.1/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-08 19:21:08.075572 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-08 19:21:08.055572 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-08 19:21:08.087573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-08 19:21:08.107573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-08 19:21:08.119573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.315375 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-08 19:21:08.135573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:56.831367 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-08 19:21:08.151574 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-08 19:21:08.163574 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-08 19:21:08.247575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-08 19:21:08.203575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-08 19:21:08.231575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-08 19:21:08.263576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-08 19:21:08.279576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 19:20:56.923369 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-08 19:21:08.291576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 19:20:56.843367 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-08 19:21:08.311577 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-08 19:21:08.319577 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-08 19:21:08.335577 windmill_api-1.96.1/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-08 19:21:08.411579 windmill_api-1.96.1/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-08 19:21:08.471579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-08 19:21:08.439579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-08 19:21:08.467579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-08 19:20:56.895368 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-08 19:21:08.495580 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-08 19:21:08.507580 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-08 19:21:08.575581 windmill_api-1.96.1/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-08 19:21:08.535581 windmill_api-1.96.1/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-08 19:21:08.563581 windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-08 19:21:08.591582 windmill_api-1.96.1/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-08 19:21:08.611582 windmill_api-1.96.1/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-08 19:20:57.591380 windmill_api-1.96.1/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-08 19:21:08.679583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-08 19:21:08.639582 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-08 19:21:08.667583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-08 19:20:57.227374 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-08 19:21:08.695583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-08 19:21:08.715584 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-08 19:20:57.083371 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-08 19:21:08.795585 windmill_api-1.96.1/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-08 19:21:08.755585 windmill_api-1.96.1/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-08 19:21:08.891587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-08 19:21:08.835586 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 19:21:08.863587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 19:21:08.899587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 19:21:08.919587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 19:21:08.931588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 19:20:57.475378 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 19:21:08.951588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 19:21:08.963588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 19:21:09.031590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 19:21:08.999589 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 19:21:09.031590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 19:21:09.063590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 19:21:09.059590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 19:20:57.083371 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 19:21:09.091591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 19:20:57.275375 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 19:21:09.095591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 19:21:09.123591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-08 19:21:09.123591 windmill_api-1.96.1/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-08 19:21:09.147592 windmill_api-1.96.1/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-08 19:21:09.151592 windmill_api-1.96.1/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-08 19:21:09.199592 windmill_api-1.96.1/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-08 19:21:09.183592 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-08 19:21:09.211593 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-08 19:20:57.319375 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-08 19:21:09.339595 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-08 19:21:09.251593 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 19:21:09.327595 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 19:21:09.363596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 19:21:09.367596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 19:20:56.743365 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 19:21:09.391596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 19:20:57.691382 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 19:21:09.399596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 19:21:09.419597 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-08 19:20:56.927368 windmill_api-1.96.1/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-08 19:21:09.455597 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:57.715382 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-08 19:21:09.443597 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-08 19:21:09.491598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-08 19:21:09.479598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-08 19:21:09.503598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-08 19:21:09.551599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-08 19:20:57.555379 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-08 19:21:09.527598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-08 19:21:09.575599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-08 19:20:57.139372 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-08 19:21:09.579599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-08 19:21:09.595600 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-08 19:21:09.627600 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-08 19:20:57.175373 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-08 19:21:09.619600 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-08 19:21:09.723602 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-08 19:20:57.479378 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-08 19:21:09.655601 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-08 19:21:09.723602 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-08 19:21:09.771603 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-08 19:20:57.327376 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-08 19:20:57.611380 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-08 19:21:09.747602 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-08 19:21:09.887605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-08 19:21:09.791603 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-08 19:21:09.831604 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-08 19:21:09.915605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-08 19:21:09.915605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-08 19:21:09.943606 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-08 19:20:56.983369 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 19:21:09.943606 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-08 19:21:09.975607 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-08 19:21:10.035608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-08 19:21:10.003607 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 19:21:10.027608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 19:20:57.211373 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 19:21:10.115609 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 19:21:10.071608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 19:20:56.983369 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-08 19:21:10.175610 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-08 19:20:56.999370 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-08 19:21:10.159610 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-08 19:21:10.239611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-08 19:21:10.215611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-08 19:21:10.243611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-08 19:21:10.267612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-08 19:21:10.275612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-08 19:21:10.295612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-08 19:20:57.639381 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-08 19:21:10.307613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-08 19:21:10.323613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-08 19:21:10.395614 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-08 19:21:10.363613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 19:21:10.391614 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 19:21:10.423615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 19:21:10.431615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.303375 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 19:21:10.503616 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.175373 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 19:21:10.467615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 19:21:10.499616 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-08 19:21:10.655619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-08 19:21:10.523616 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-08 19:21:10.543617 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-08 19:21:10.583617 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-08 19:21:10.663619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-08 19:21:10.695619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 19:21:10.691619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 19:21:10.723620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 19:21:10.727620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 19:20:56.691365 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 19:21:10.751620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 19:20:56.759366 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 19:21:10.759621 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 19:21:10.779621 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-08 19:21:10.843622 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-08 19:21:10.819622 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-08 19:21:10.895623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-08 19:21:10.875623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-08 19:21:10.907623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 19:20:56.703365 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-08 19:21:10.923623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-08 19:21:10.935624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-08 19:21:10.951624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-08 19:21:10.967624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-08 19:21:11.019625 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-08 19:21:11.059626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-08 19:21:11.039626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-08 19:21:11.083626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-08 19:21:11.147627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-08 19:21:11.119627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-08 19:21:11.147627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-08 19:21:11.183628 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-08 19:21:11.179628 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-08 19:20:56.919368 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-08 19:21:11.207629 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-08 19:20:57.019370 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-08 19:21:11.211629 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-08 19:21:11.291630 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-08 19:21:11.299630 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-08 19:21:11.335631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-08 19:21:11.331631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-08 19:21:11.367632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-08 19:21:11.363631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-08 19:20:56.871368 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-08 19:21:11.391632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-08 19:20:57.739382 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-08 19:21:11.395632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-08 19:21:11.419633 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-08 19:21:11.503634 windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-08 19:21:11.439633 windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-08 19:21:11.471633 windmill_api-1.96.1/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-08 19:21:11.491634 windmill_api-1.96.1/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-08 19:21:11.527634 windmill_api-1.96.1/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      325 2023-05-08 19:20:56.931369 windmill_api-1.96.1/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-08 19:21:11.523634 windmill_api-1.96.1/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-08 19:21:11.571635 windmill_api-1.96.1/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-08 19:21:11.547635 windmill_api-1.96.1/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-08 19:21:11.567635 windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-08 19:21:11.595636 windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-08 19:21:11.603636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-08 19:21:11.635636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-08 19:21:11.623636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-08 19:21:11.667637 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-08 19:21:11.767639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-08 19:21:11.707638 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-08 19:21:11.735638 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-08 19:21:11.771639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-08 19:21:11.795639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.475378 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-08 19:21:11.799639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:56.979369 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-08 19:21:11.823640 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-08 19:21:11.831640 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-08 19:21:11.907641 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-08 19:21:11.943642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-08 19:21:11.935642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-08 19:21:11.967642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-08 19:21:11.975642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-08 19:20:57.783383 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-08 19:21:11.995643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 19:21:12.007643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-08 19:21:12.023643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-08 19:21:12.047644 windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-08 19:20:57.723382 windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-08 19:21:12.063644 windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-08 19:21:12.067644 windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-08 19:20:57.079371 windmill_api-1.96.1/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-08 19:21:12.159646 windmill_api-1.96.1/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-08 19:20:57.259374 windmill_api-1.96.1/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-08 19:21:12.107645 windmill_api-1.96.1/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-08 19:21:12.135645 windmill_api-1.96.1/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-08 19:21:12.191646 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-08 19:21:12.183646 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-08 19:21:12.231647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-08 19:20:57.147372 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-08 19:21:12.219647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-08 19:21:12.239647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-08 19:21:12.279648 windmill_api-1.96.1/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.259647 windmill_api-1.96.1/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-08 19:21:12.371650 windmill_api-1.96.1/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-08 19:21:12.307648 windmill_api-1.96.1/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-08 19:21:12.367649 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:12.387650 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.391650 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-08 19:21:12.479652 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 19:21:12.411650 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 19:20:57.775383 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 19:20:57.239374 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.439651 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-08 19:21:12.531652 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 19:21:12.571653 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.555653 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-08 19:21:12.639654 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-08 19:21:12.643654 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-08 19:20:57.751383 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-08 19:21:12.667655 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-08 19:20:57.735382 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-08 19:21:12.671655 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-08 19:21:12.695655 windmill_api-1.96.1/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-08 19:21:12.811658 windmill_api-1.96.1/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-08 19:21:12.727656 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-08 19:21:12.755656 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-08 19:21:12.783657 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-08 19:20:56.767366 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-08 19:21:12.847658 windmill_api-1.96.1/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.831658 windmill_api-1.96.1/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-08 19:21:12.875659 windmill_api-1.96.1/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-08 19:21:12.871658 windmill_api-1.96.1/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-08 19:21:12.911659 windmill_api-1.96.1/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:20:56.875368 windmill_api-1.96.1/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-08 19:21:12.919659 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-08 19:21:13.039662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-08 19:20:57.219374 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-08 19:21:12.947660 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-08 19:21:12.971660 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-08 19:21:13.003661 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-08 19:21:13.043662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-08 19:20:56.719365 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-08 19:21:13.063662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-08 19:21:13.079662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 19:21:13.091663 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.127372 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-08 19:21:13.127663 windmill_api-1.96.1/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-08 19:21:13.111663 windmill_api-1.96.1/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-08 19:21:13.139663 windmill_api-1.96.1/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-08 19:20:57.011370 windmill_api-1.96.1/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 19:21:13.171664 windmill_api-1.96.1/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-08 19:21:13.159664 windmill_api-1.96.1/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-08 19:21:13.187664 windmill_api-1.96.1/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-08 19:21:13.275666 windmill_api-1.96.1/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:57.615380 windmill_api-1.96.1/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 19:21:13.219665 windmill_api-1.96.1/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-08 19:21:13.243665 windmill_api-1.96.1/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-08 19:20:57.163373 windmill_api-1.96.1/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-08 19:21:13.275666 windmill_api-1.96.1/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-08 19:20:57.651381 windmill_api-1.96.1/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-08 19:21:13.323667 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:56.851367 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-08 19:21:13.299666 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-08 19:21:13.411668 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-08 19:20:57.723382 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-08 19:20:57.279374 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-08 19:21:13.351667 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-08 19:21:13.491670 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-08 19:21:13.431669 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-08 19:21:13.475669 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-08 19:21:13.559671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-08 19:21:13.515670 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-08 19:21:13.543671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-08 19:20:56.967369 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-08 19:21:13.575671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-08 19:21:13.595672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-08 19:21:13.751674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-08 19:21:13.623672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-08 19:21:13.651672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-08 19:20:57.055371 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-08 19:21:13.675673 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-08 19:21:13.711674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-08 19:20:57.227374 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-08 19:21:13.743674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-08 19:20:57.615380 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:57.223374 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-08 19:21:13.863676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-08 19:21:13.835676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-08 19:21:13.875676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-08 19:21:13.891677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-08 19:21:13.911677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-08 19:21:13.919677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-08 19:20:56.683364 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-08 19:21:13.939678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-08 19:20:57.347376 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 19:21:13.947678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-08 19:21:13.971678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-08 19:21:14.031679 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-08 19:21:14.015679 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-08 19:21:14.043680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-08 19:21:14.063680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-08 19:21:14.075680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-08 19:20:56.703365 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-08 19:21:14.091680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-08 19:20:57.023370 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-08 19:21:14.187682 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-08 19:21:14.119681 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-08 19:21:14.151682 windmill_api-1.96.1/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-08 19:21:14.255683 windmill_api-1.96.1/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-08 19:21:14.231683 windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 19:21:14.251683 windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-08 19:21:14.299684 windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-08 19:21:14.275683 windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-08 19:21:14.307684 windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-08 19:21:14.335685 windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 19:21:14.339685 windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-08 19:21:14.371685 windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 19:21:14.371685 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-08 19:21:14.407686 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-08 19:20:57.403377 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-08 19:21:14.411686 windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-08 19:21:14.431686 windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 19:21:14.443687 windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-08 19:20:56.683364 windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-08 19:21:14.463687 windmill_api-1.96.1/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-08 19:21:14.691691 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-08 19:21:14.483687 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-08 19:21:14.567689 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-08 19:21:14.743692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-08 19:21:14.715691 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 19:21:14.747692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 19:20:57.787383 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 19:21:14.771692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 19:21:14.783692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 19:20:57.359376 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-08 19:21:14.855694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-08 19:21:14.807693 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-08 19:21:14.839694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-08 19:20:57.599380 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-08 19:21:14.867694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-08 19:21:14.891694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-08 19:21:14.903695 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-08 19:20:57.795383 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-08 19:20:57.251374 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-08 19:21:14.935695 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-08 19:21:14.987696 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-08 19:21:14.975696 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 19:21:15.079698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 19:21:15.019697 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 19:21:15.047697 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.459378 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 19:21:15.079698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.099372 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 19:21:15.183700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 19:21:15.107698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-08 19:21:15.191700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-08 19:21:15.227700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 19:21:15.219700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 19:21:15.251701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 19:21:15.255701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 19:20:57.251374 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 19:21:15.279701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 19:20:56.987370 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 19:21:15.287701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 19:21:15.307702 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3045 2023-05-08 19:21:15.331702 windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item.py
+-rw-r--r--   0        0        0     1294 2023-05-08 19:21:15.327702 windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     4884 2023-05-08 19:21:15.391703 windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 19:21:15.351703 windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-08 19:21:15.387703 windmill_api-1.96.1/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-08 19:21:15.443704 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-08 19:21:15.479705 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-08 19:21:15.463704 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-08 19:21:15.631708 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 19:21:15.499705 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 19:20:57.543379 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 19:20:57.539379 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-08 19:21:15.523706 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-08 19:21:15.563706 windmill_api-1.96.1/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-08 19:21:15.591707 windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-08 19:21:15.623707 windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-08 19:21:15.659708 windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-08 19:20:57.559379 windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-08 19:21:15.703709 windmill_api-1.96.1/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-08 19:21:15.683709 windmill_api-1.96.1/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-08 19:21:15.779710 windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 19:21:15.735709 windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-08 19:21:15.779710 windmill_api-1.96.1/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 19:21:15.811711 windmill_api-1.96.1/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-08 19:21:15.815711 windmill_api-1.96.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-08 19:21:15.847711 windmill_api-1.96.1/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-08 19:21:15.859712 windmill_api-1.96.1/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-08 19:20:57.343376 windmill_api-1.96.1/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-08 19:21:15.867712 windmill_api-1.96.1/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     2913 2023-05-08 19:21:15.899712 windmill_api-1.96.1/windmill_api/models/listable_raw_app.py
+-rw-r--r--   0        0        0     1225 2023-05-08 19:21:15.887712 windmill_api-1.96.1/windmill_api/models/listable_raw_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-08 19:21:15.955713 windmill_api-1.96.1/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:15.919713 windmill_api-1.96.1/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-08 19:21:16.055715 windmill_api-1.96.1/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:15.975714 windmill_api-1.96.1/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-08 19:21:15.999714 windmill_api-1.96.1/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-08 19:21:16.027715 windmill_api-1.96.1/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-08 19:21:16.127716 windmill_api-1.96.1/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-08 19:21:16.095716 windmill_api-1.96.1/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-08 19:21:16.151717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-08 19:20:57.367376 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-08 19:21:16.155717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-08 19:21:16.179717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-08 19:21:16.183717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-08 19:21:16.215718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-08 19:20:56.815367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 19:21:16.211718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-08 19:21:16.247718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-08 19:20:56.851367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-08 19:21:16.239718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 19:20:56.815367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-08 19:21:16.279719 windmill_api-1.96.1/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-08 19:21:16.263719 windmill_api-1.96.1/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-08 19:21:16.339720 windmill_api-1.96.1/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-08 19:20:57.407377 windmill_api-1.96.1/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.567380 windmill_api-1.96.1/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-08 19:21:16.303719 windmill_api-1.96.1/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-08 19:21:16.467722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-08 19:21:16.411721 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-08 19:20:57.027370 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-08 19:20:57.099372 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-08 19:21:16.435722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-08 19:20:56.739365 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-08 19:20:57.095371 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-08 19:21:16.455722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-08 19:21:16.567724 windmill_api-1.96.1/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-08 19:21:16.503723 windmill_api-1.96.1/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-08 19:21:16.531723 windmill_api-1.96.1/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-08 19:21:16.571724 windmill_api-1.96.1/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 19:21:16.591724 windmill_api-1.96.1/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-08 19:21:16.611725 windmill_api-1.96.1/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-08 19:21:16.671726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-08 19:21:16.651725 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-08 19:21:16.679726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-08 19:21:16.703726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-08 19:21:16.703726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-08 19:21:16.731727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-08 19:20:57.635381 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-08 19:21:16.731727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-08 19:21:16.759727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-08 19:21:16.899730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-08 19:21:16.799728 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-08 19:21:16.827729 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-08 19:21:16.859729 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-08 19:21:16.887730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 19:20:57.427377 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-08 19:21:16.999732 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-08 19:21:16.931730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-08 19:21:16.959731 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-08 19:21:17.003732 windmill_api-1.96.1/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-08 19:21:17.023732 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-08 19:21:17.043733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-08 19:21:17.103733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-08 19:21:17.083733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-08 19:21:17.111734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-08 19:21:17.135734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-08 19:21:17.139734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-08 19:20:56.923369 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-08 19:21:17.163735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 19:20:56.887368 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-08 19:21:17.171735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-08 19:21:17.191735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-08 19:21:17.247736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-08 19:21:17.231736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-08 19:21:17.259736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-08 19:21:17.283737 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-08 19:21:17.379738 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-08 19:21:17.311737 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.739382 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-08 19:21:17.435739 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-08 19:21:17.407739 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-08 19:21:17.435739 windmill_api-1.96.1/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-08 19:21:17.471740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-08 19:21:17.463740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:20:56.959369 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-08 19:21:17.491740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:20:56.811367 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-08 19:20:57.011370 windmill_api-1.96.1/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-08 19:21:17.507741 windmill_api-1.96.1/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-08 19:21:17.527741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-08 19:21:17.539741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 19:20:57.663381 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 19:21:17.555741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 19:20:57.263374 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-08 19:21:17.591742 windmill_api-1.96.1/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-08 19:20:57.755383 windmill_api-1.96.1/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-08 19:21:17.579742 windmill_api-1.96.1/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-08 19:21:17.599742 windmill_api-1.96.1/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-08 19:21:17.631743 windmill_api-1.96.1/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-08 19:21:17.619742 windmill_api-1.96.1/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-08 19:20:57.587380 windmill_api-1.96.1/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-08 19:21:17.647743 windmill_api-1.96.1/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-08 19:21:17.671743 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-08 19:21:17.707744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-08 19:20:56.819367 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-08 19:21:17.699744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-08 19:21:17.727744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-08 19:21:17.731745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-08 19:21:17.767745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-08 19:21:17.755745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-08 19:21:17.883747 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-08 19:20:56.699365 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-08 19:21:17.791746 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-08 19:20:57.683381 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-08 19:21:18.035750 windmill_api-1.96.1/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-08 19:21:17.899747 windmill_api-1.96.1/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-08 19:21:17.943748 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-08 19:21:18.023750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-08 19:21:18.051750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 19:21:18.063750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-08 19:21:18.075751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-08 19:21:18.099751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-08 19:21:18.155752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-08 19:21:18.123751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 19:21:18.151752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-08 19:21:18.183752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-08 19:21:18.279754 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-08 19:20:56.691365 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-08 19:21:18.215753 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-08 19:20:57.571380 windmill_api-1.96.1/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-08 19:21:18.259754 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-08 19:21:18.447757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-08 19:21:18.315755 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-08 19:21:18.347755 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-08 19:21:18.379756 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-08 19:21:18.407756 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.419377 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 19:21:18.431757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 19:20:57.347376 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 19:21:18.459757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-08 19:21:18.475758 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-08 19:21:18.535759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-08 19:21:18.511758 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-08 19:21:18.543759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-08 19:21:18.567759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-08 19:21:18.571759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-08 19:21:18.595760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 19:20:57.239374 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-08 19:21:18.599760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-08 19:21:18.623760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-08 19:21:18.643761 windmill_api-1.96.1/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-08 19:21:18.655761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-08 19:21:18.675761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-08 19:20:57.259374 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-08 19:21:18.683761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-08 19:20:57.199373 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-08 19:20:57.675381 windmill_api-1.96.1/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-08 19:20:56.711365 windmill_api-1.96.1/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-08 19:21:18.703762 windmill_api-1.96.1/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-08 19:21:18.703762 windmill_api-1.96.1/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      328 2023-05-08 19:20:57.075371 windmill_api-1.96.1/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-08 19:21:18.823764 windmill_api-1.96.1/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-08 19:21:18.731762 windmill_api-1.96.1/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-08 19:21:18.863764 windmill_api-1.96.1/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-08 19:21:18.839764 windmill_api-1.96.1/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-08 19:21:18.875765 windmill_api-1.96.1/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-08 19:21:18.883765 windmill_api-1.96.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 19:21:18.899765 windmill_api-1.96.1/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-08 19:21:18.923766 windmill_api-1.96.1/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-08 19:21:18.927766 windmill_api-1.96.1/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-08 19:21:18.955766 windmill_api-1.96.1/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-08 19:21:18.947766 windmill_api-1.96.1/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-08 19:21:18.983767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-08 19:21:18.975767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 19:21:19.015767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-08 19:21:19.063768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-08 19:21:19.055768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-08 19:21:19.083768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-08 19:21:19.099769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-08 19:21:19.111769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 19:20:56.859367 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 19:21:19.127769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 19:20:56.803367 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-08 19:21:19.139769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-08 19:21:19.159770 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-08 19:21:19.219771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-08 19:21:19.203770 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-08 19:21:19.235771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-08 19:21:19.251771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-08 19:21:19.355773 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 19:20:57.619380 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-08 19:21:19.371773 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 19:20:57.451377 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-08 19:21:19.383774 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-08 19:21:19.399774 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-08 19:21:19.403774 windmill_api-1.96.1/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-08 19:21:19.419774 windmill_api-1.96.1/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-08 19:21:19.443775 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-08 19:21:19.439775 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-08 19:20:57.539379 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-08 19:21:19.459775 windmill_api-1.96.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-08 19:21:19.463775 windmill_api-1.96.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-08 19:20:57.491378 windmill_api-1.96.1/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-08 19:21:19.519776 windmill_api-1.96.1/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-08 19:21:19.483775 windmill_api-1.96.1/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-08 19:21:19.503776 windmill_api-1.96.1/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-08 19:21:19.599778 windmill_api-1.96.1/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-08 19:21:19.535776 windmill_api-1.96.1/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-08 19:21:19.555777 windmill_api-1.96.1/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-08 19:20:57.415377 windmill_api-1.96.1/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-08 19:20:57.627380 windmill_api-1.96.1/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-08 19:21:19.579777 windmill_api-1.96.1/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-08 19:21:19.599778 windmill_api-1.96.1/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-08 19:21:19.623778 windmill_api-1.96.1/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-08 19:21:19.631778 windmill_api-1.96.1/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-08 19:21:19.647778 windmill_api-1.96.1/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-08 19:21:19.663779 windmill_api-1.96.1/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      209 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-08 19:21:19.679779 windmill_api-1.96.1/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-08 19:20:57.327376 windmill_api-1.96.1/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-08 19:21:19.703779 windmill_api-1.96.1/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-08 19:21:19.719780 windmill_api-1.96.1/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-08 19:21:19.735780 windmill_api-1.96.1/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      211 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-08 19:21:19.763780 windmill_api-1.96.1/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 19:21:19.779781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 19:20:57.155372 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 19:21:19.791781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 19:21:19.799781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-08 19:21:19.935783 windmill_api-1.96.1/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-08 19:21:19.819781 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-08 19:21:19.859782 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-08 19:21:20.043785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-08 19:21:19.975784 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-08 19:21:20.007785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-08 19:21:20.039785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-08 19:21:20.067786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:20:57.519379 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-08 19:21:20.071786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-08 19:21:20.099786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-08 19:21:20.099786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-08 19:21:20.179788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-08 19:21:20.139787 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-08 19:21:20.171788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-08 19:21:20.199788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-08 19:21:20.207788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-08 19:20:57.235374 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-08 19:21:20.227789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-08 19:20:57.423377 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-08 19:21:20.239789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-08 19:21:20.255789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-08 19:21:20.375791 windmill_api-1.96.1/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-08 19:21:20.283789 windmill_api-1.96.1/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-08 19:21:20.307790 windmill_api-1.96.1/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-08 19:21:20.335790 windmill_api-1.96.1/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     1985 2023-05-08 19:21:20.367791 windmill_api-1.96.1/windmill_api/models/update_raw_app_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-08 19:21:20.399792 windmill_api-1.96.1/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-08 19:21:20.403792 windmill_api-1.96.1/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-08 19:21:20.423792 windmill_api-1.96.1/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-08 19:21:20.435792 windmill_api-1.96.1/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 19:21:20.447792 windmill_api-1.96.1/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-08 19:21:20.467793 windmill_api-1.96.1/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-08 19:21:20.479793 windmill_api-1.96.1/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-08 19:21:20.495793 windmill_api-1.96.1/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-08 19:21:20.659796 windmill_api-1.96.1/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-08 19:21:20.523794 windmill_api-1.96.1/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-08 19:21:20.551794 windmill_api-1.96.1/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-08 19:21:20.583795 windmill_api-1.96.1/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-08 19:21:20.643796 windmill_api-1.96.1/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-08 19:21:20.671796 windmill_api-1.96.1/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-08 19:21:20.719797 windmill_api-1.96.1/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-08 19:21:20.691797 windmill_api-1.96.1/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-08 19:21:20.731797 windmill_api-1.96.1/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-08 19:21:20.751798 windmill_api-1.96.1/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-08 19:21:20.763798 windmill_api-1.96.1/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-08 19:20:47.203207 windmill_api-1.96.1/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-08 19:21:20.767798 windmill_api-1.96.1/windmill_api/types.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.1/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.1/PKG-INFO
```

### Comparing `windmill_api-1.96.0/LICENSE` & `windmill_api-1.96.1/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/README.md` & `windmill_api-1.96.1/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/pyproject.toml` & `windmill_api-1.96.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.96.0"
+version = "1.96.1"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.96.0/windmill_api/api/app/create_app.py` & `windmill_api-1.96.1/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.96.1/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.96.1/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.96.1/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.96.1/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.96.1/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.96.1/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.96.1/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.96.1/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.96.1/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.96.1/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.96.1/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/app/update_app.py` & `windmill_api-1.96.1/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.96.1/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.96.1/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.96.1/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.96.1/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.96.1/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/draft/create_draft.py` & `windmill_api-1.96.1/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/favorite/star.py` & `windmill_api-1.96.1/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.96.1/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.96.1/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.96.1/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.96.1/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.96.1/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.96.1/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.96.1/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.96.1/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.96.1/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.96.1/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.96.1/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.96.1/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.96.1/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.96.1/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.96.1/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.96.1/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/create_group.py` & `windmill_api-1.96.1/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.96.1/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/get_group.py` & `windmill_api-1.96.1/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.96.1/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.96.1/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.96.1/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/group/update_group.py` & `windmill_api-1.96.1/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/input_/create_input.py` & `windmill_api-1.96.1/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/input_/delete_input.py` & `windmill_api-1.96.1/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.96.1/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.96.1/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/input_/update_input.py` & `windmill_api-1.96.1/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.96.1/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.96.1/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.96.1/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.96.1/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.96.1/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.96.1/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_job.py` & `windmill_api-1.96.1/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.96.1/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.96.1/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.96.1/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.96.1/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.96.1/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.96.1/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.96.1/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.96.1/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.96.1/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.96.1/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.96.1/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.96.1/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.96.1/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.96.1/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.96.1/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.96.1/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/create_raw_app.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/create_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/delete_raw_app.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/delete_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/exists_raw_app.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/exists_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/get_raw_app_data.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/get_raw_app_data.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/list_raw_apps.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/list_raw_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/raw_app/update_raw_app.py` & `windmill_api-1.96.1/windmill_api/api/raw_app/update_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.96.1/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.96.1/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.96.1/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.96.1/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.96.1/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.96.1/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.96.1/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.96.1/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.96.1/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.96.1/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/create_script.py` & `windmill_api-1.96.1/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.96.1/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.96.1/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.96.1/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.96.1/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.96.1/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.96.1/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.96.1/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.96.1/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.96.1/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.96.1/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.96.1/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.96.1/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.96.1/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/create_token.py` & `windmill_api-1.96.1/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.96.1/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/create_user.py` & `windmill_api-1.96.1/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.96.1/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.96.1/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.96.1/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.96.1/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.96.1/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.96.1/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.96.1/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.96.1/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.96.1/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.96.1/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.96.1/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.96.1/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.96.1/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/list_users.py` & `windmill_api-1.96.1/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.96.1/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.96.1/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/login.py` & `windmill_api-1.96.1/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.96.1/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/logout.py` & `windmill_api-1.96.1/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/set_password.py` & `windmill_api-1.96.1/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/update_user.py` & `windmill_api-1.96.1/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/whoami.py` & `windmill_api-1.96.1/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/user/whois.py` & `windmill_api-1.96.1/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.96.1/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.96.1/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.96.1/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.96.1/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.96.1/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.96.1/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.96.1/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.96.1/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.96.1/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.96.1/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.96.1/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.96.1/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.96.1/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.96.1/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.96.1/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.96.1/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.96.1/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.96.1/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.96.1/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.96.1/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.96.1/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/client.py` & `windmill_api-1.96.1/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.96.1/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.96.1/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.96.1/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.96.1/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.96.1/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.96.1/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/audit_log.py` & `windmill_api-1.96.1/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.96.1/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.96.1/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all.py` & `windmill_api-1.96.1/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one.py` & `windmill_api-1.96.1/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.96.1/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.96.1/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job.py` & `windmill_api-1.96.1/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.96.1/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.96.1/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.96.1/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.96.1/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_input.py` & `windmill_api-1.96.1/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_input_args.py` & `windmill_api-1.96.1/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_input_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.96.1/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_raw_app_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_resource.py` & `windmill_api-1.96.1/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.96.1/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.96.1/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_variable.py` & `windmill_api-1.96.1/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_workspace.py` & `windmill_api-1.96.1/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.96.1/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.96.1/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.96.1/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.96.1/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_resource.py` & `windmill_api-1.96.1/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.96.1/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.96.1/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.96.1/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.96.1/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_variable.py` & `windmill_api-1.96.1/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.96.1/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.96.1/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.96.1/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.96.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.96.1/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.96.1/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.96.1/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow.py` & `windmill_api-1.96.1/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.96.1/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module.py` & `windmill_api-1.96.1/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_schema.py` & `windmill_api-1.96.1/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status.py` & `windmill_api-1.96.1/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value.py` & `windmill_api-1.96.1/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/folder.py` & `windmill_api-1.96.1/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.96.1/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.96.1/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/global_user_info.py` & `windmill_api-1.96.1/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.96.1/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.96.1/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/group.py` & `windmill_api-1.96.1/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/identity.py` & `windmill_api-1.96.1/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/input_.py` & `windmill_api-1.96.1/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/input_args.py` & `windmill_api-1.96.1/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.96.1/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.96.1/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.96.1/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.96.1/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/job.py` & `windmill_api-1.96.1/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.96.1/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.96.1/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_app.py` & `windmill_api-1.96.1/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_raw_app.py` & `windmill_api-1.96.1/windmill_api/models/listable_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_raw_app_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/listable_raw_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_resource.py` & `windmill_api-1.96.1/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_variable.py` & `windmill_api-1.96.1/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/login.py` & `windmill_api-1.96.1/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/login_json_body.py` & `windmill_api-1.96.1/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.96.1/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_schedule.py` & `windmill_api-1.96.1/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.96.1/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script.py` & `windmill_api-1.96.1/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script_schema.py` & `windmill_api-1.96.1/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.96.1/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_token.py` & `windmill_api-1.96.1/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.96.1/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/new_user.py` & `windmill_api-1.96.1/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow.py` & `windmill_api-1.96.1/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_flow.py` & `windmill_api-1.96.1/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_script.py` & `windmill_api-1.96.1/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/policy.py` & `windmill_api-1.96.1/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/preview.py` & `windmill_api-1.96.1/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/preview_args.py` & `windmill_api-1.96.1/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.96.1/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job.py` & `windmill_api-1.96.1/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/raw_script.py` & `windmill_api-1.96.1/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.96.1/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.96.1/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.96.1/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.96.1/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/resource.py` & `windmill_api-1.96.1/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/resource_type.py` & `windmill_api-1.96.1/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.96.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.96.1/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/retry.py` & `windmill_api-1.96.1/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.96.1/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/schedule.py` & `windmill_api-1.96.1/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/schedule_args.py` & `windmill_api-1.96.1/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/script.py` & `windmill_api-1.96.1/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/script_args.py` & `windmill_api-1.96.1/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.96.1/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/script_schema.py` & `windmill_api-1.96.1/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.96.1/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.96.1/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/slack_token.py` & `windmill_api-1.96.1/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.96.1/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/star_json_body.py` & `windmill_api-1.96.1/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/static_transform.py` & `windmill_api-1.96.1/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/token_response.py` & `windmill_api-1.96.1/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/truncated_token.py` & `windmill_api-1.96.1/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.96.1/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_input.py` & `windmill_api-1.96.1/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_input_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_raw_app_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.96.1/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_user_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.96.1/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/usage.py` & `windmill_api-1.96.1/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/user.py` & `windmill_api-1.96.1/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/user_usage.py` & `windmill_api-1.96.1/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.96.1/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.96.1/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.96.1/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.96.1/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.96.1/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.96.1/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/worker_ping.py` & `windmill_api-1.96.1/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/workspace.py` & `windmill_api-1.96.1/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/models/workspace_invite.py` & `windmill_api-1.96.1/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/windmill_api/types.py` & `windmill_api-1.96.1/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.0/setup.py` & `windmill_api-1.96.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.96.0',
+    'version': '1.96.1',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.96.0/PKG-INFO` & `windmill_api-1.96.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.96.0
+Version: 1.96.1
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


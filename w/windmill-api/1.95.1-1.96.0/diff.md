# Comparing `tmp/windmill_api-1.95.1.tar.gz` & `tmp/windmill_api-1.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.95.1.tar", max compression
+gzip compressed data, was "windmill_api-1.96.0.tar", max compression
```

## Comparing `windmill_api-1.95.1.tar` & `windmill_api-1.96.0.tar`

### file list

```diff
@@ -1,1289 +1,1302 @@
--rw-r--r--   0        0        0    11348 2023-05-06 10:11:34.669474 windmill_api-1.95.1/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-06 10:11:34.673474 windmill_api-1.95.1/README.md
--rw-r--r--   0        0        0      717 2023-05-06 10:11:34.673474 windmill_api-1.95.1/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-06 10:11:01.929416 windmill_api-1.95.1/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-06 10:11:02.413417 windmill_api-1.95.1/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.521417 windmill_api-1.95.1/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-06 10:11:13.217443 windmill_api-1.95.1/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-06 10:11:13.229443 windmill_api-1.95.1/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-06 10:11:13.265443 windmill_api-1.95.1/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-06 10:11:13.269443 windmill_api-1.95.1/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-06 10:11:13.309443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-06 10:11:13.313443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-06 10:11:13.349443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-06 10:11:13.361443 windmill_api-1.95.1/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-06 10:11:13.409443 windmill_api-1.95.1/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-06 10:11:13.393443 windmill_api-1.95.1/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-06 10:11:13.489444 windmill_api-1.95.1/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-06 10:11:13.441444 windmill_api-1.95.1/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-06 10:11:13.473444 windmill_api-1.95.1/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.453417 windmill_api-1.95.1/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-06 10:11:13.517444 windmill_api-1.95.1/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-06 10:11:13.605444 windmill_api-1.95.1/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.585417 windmill_api-1.95.1/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-06 10:11:13.545444 windmill_api-1.95.1/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-06 10:11:13.573444 windmill_api-1.95.1/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-06 10:11:13.601444 windmill_api-1.95.1/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.541417 windmill_api-1.95.1/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-06 10:11:13.633444 windmill_api-1.95.1/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.589418 windmill_api-1.95.1/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-06 10:11:13.641444 windmill_api-1.95.1/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-06 10:11:13.661444 windmill_api-1.95.1/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.509417 windmill_api-1.95.1/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-06 10:11:13.673444 windmill_api-1.95.1/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-06 10:11:13.693444 windmill_api-1.95.1/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-06 10:11:13.705444 windmill_api-1.95.1/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-06 10:11:13.745444 windmill_api-1.95.1/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-06 10:11:13.765444 windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-06 10:11:13.785444 windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-06 10:11:13.829445 windmill_api-1.95.1/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-06 10:11:13.825444 windmill_api-1.95.1/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-06 10:11:13.853444 windmill_api-1.95.1/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-06 10:11:13.933445 windmill_api-1.95.1/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-06 10:11:13.885444 windmill_api-1.95.1/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-06 10:11:13.917445 windmill_api-1.95.1/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.577417 windmill_api-1.95.1/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-06 10:11:13.949445 windmill_api-1.95.1/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-06 10:11:13.965445 windmill_api-1.95.1/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-06 10:11:13.977445 windmill_api-1.95.1/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-06 10:11:14.009445 windmill_api-1.95.1/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-06 10:11:14.017445 windmill_api-1.95.1/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-06 10:11:14.061445 windmill_api-1.95.1/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-06 10:11:14.093445 windmill_api-1.95.1/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-06 10:11:14.097445 windmill_api-1.95.1/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-06 10:11:14.125445 windmill_api-1.95.1/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.585417 windmill_api-1.95.1/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-06 10:11:14.149445 windmill_api-1.95.1/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-06 10:11:14.173445 windmill_api-1.95.1/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-06 10:11:14.181445 windmill_api-1.95.1/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.573417 windmill_api-1.95.1/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-06 10:11:14.209445 windmill_api-1.95.1/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-06 10:11:14.209445 windmill_api-1.95.1/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-06 10:11:14.237445 windmill_api-1.95.1/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-06 10:11:14.253445 windmill_api-1.95.1/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-06 10:11:14.289445 windmill_api-1.95.1/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-06 10:11:14.317446 windmill_api-1.95.1/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-06 10:11:14.317446 windmill_api-1.95.1/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-06 10:11:14.349446 windmill_api-1.95.1/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.589418 windmill_api-1.95.1/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-06 10:11:14.365446 windmill_api-1.95.1/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-06 10:11:14.377446 windmill_api-1.95.1/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-06 10:11:14.461446 windmill_api-1.95.1/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-06 10:11:14.449446 windmill_api-1.95.1/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-06 10:11:14.497446 windmill_api-1.95.1/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.545417 windmill_api-1.95.1/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-06 10:11:14.493446 windmill_api-1.95.1/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-06 10:11:14.537446 windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-06 10:11:14.541446 windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-06 10:11:14.577446 windmill_api-1.95.1/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-06 10:11:14.581446 windmill_api-1.95.1/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-06 10:11:14.609446 windmill_api-1.95.1/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-06 10:11:14.621446 windmill_api-1.95.1/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:14.637446 windmill_api-1.95.1/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-06 10:11:14.661446 windmill_api-1.95.1/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-06 10:11:14.697446 windmill_api-1.95.1/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-06 10:11:14.721446 windmill_api-1.95.1/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-06 10:11:14.757446 windmill_api-1.95.1/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-06 10:11:14.889447 windmill_api-1.95.1/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-06 10:11:14.917447 windmill_api-1.95.1/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-06 10:11:15.045447 windmill_api-1.95.1/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-06 10:11:14.949447 windmill_api-1.95.1/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-06 10:11:14.981447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-06 10:11:15.029447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-06 10:11:15.073447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-06 10:11:15.101447 windmill_api-1.95.1/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-06 10:11:15.117447 windmill_api-1.95.1/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-06 10:11:15.161447 windmill_api-1.95.1/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-06 10:11:15.193447 windmill_api-1.95.1/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-06 10:11:15.201447 windmill_api-1.95.1/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-06 10:11:15.237448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-06 10:11:15.273448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-06 10:11:15.289448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.485417 windmill_api-1.95.1/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-06 10:11:15.313448 windmill_api-1.95.1/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-06 10:11:15.321448 windmill_api-1.95.1/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-06 10:11:15.345448 windmill_api-1.95.1/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-06 10:11:15.353448 windmill_api-1.95.1/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-06 10:11:15.369448 windmill_api-1.95.1/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-06 10:11:15.385448 windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-06 10:11:15.405448 windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-06 10:11:15.421448 windmill_api-1.95.1/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.489417 windmill_api-1.95.1/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-06 10:11:15.437448 windmill_api-1.95.1/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-06 10:11:15.453448 windmill_api-1.95.1/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:15.465448 windmill_api-1.95.1/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-06 10:11:15.485448 windmill_api-1.95.1/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-06 10:11:15.505448 windmill_api-1.95.1/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-06 10:11:15.529448 windmill_api-1.95.1/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-06 10:11:15.545448 windmill_api-1.95.1/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-06 10:11:15.585448 windmill_api-1.95.1/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-06 10:11:15.589448 windmill_api-1.95.1/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-06 10:11:15.661449 windmill_api-1.95.1/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-06 10:11:15.629449 windmill_api-1.95.1/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-06 10:11:15.669448 windmill_api-1.95.1/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-06 10:11:15.693449 windmill_api-1.95.1/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-06 10:11:15.697449 windmill_api-1.95.1/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-06 10:11:15.729449 windmill_api-1.95.1/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.569417 windmill_api-1.95.1/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-06 10:11:15.729449 windmill_api-1.95.1/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:15.757449 windmill_api-1.95.1/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-06 10:11:15.769449 windmill_api-1.95.1/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-06 10:11:15.801449 windmill_api-1.95.1/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-06 10:11:15.829449 windmill_api-1.95.1/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-06 10:11:15.849449 windmill_api-1.95.1/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-06 10:11:15.861449 windmill_api-1.95.1/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-06 10:11:15.881449 windmill_api-1.95.1/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.497417 windmill_api-1.95.1/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-06 10:11:15.901449 windmill_api-1.95.1/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-06 10:11:15.913449 windmill_api-1.95.1/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-06 10:11:15.949449 windmill_api-1.95.1/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-06 10:11:15.957449 windmill_api-1.95.1/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-06 10:11:15.989449 windmill_api-1.95.1/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-06 10:11:16.001449 windmill_api-1.95.1/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-06 10:11:16.029449 windmill_api-1.95.1/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-06 10:11:16.045449 windmill_api-1.95.1/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-06 10:11:16.069449 windmill_api-1.95.1/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-06 10:11:16.073449 windmill_api-1.95.1/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-06 10:11:16.109449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-06 10:11:16.117449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-06 10:11:16.149449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-06 10:11:16.157450 windmill_api-1.95.1/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-06 10:11:16.189450 windmill_api-1.95.1/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-06 10:11:16.193450 windmill_api-1.95.1/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-06 10:11:16.213450 windmill_api-1.95.1/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-06 10:11:16.349450 windmill_api-1.95.1/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-06 10:11:16.269450 windmill_api-1.95.1/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.297450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.325450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-06 10:11:16.357450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.425417 windmill_api-1.95.1/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-06 10:11:16.377450 windmill_api-1.95.1/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-06 10:11:16.381450 windmill_api-1.95.1/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.457417 windmill_api-1.95.1/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-06 10:11:16.405450 windmill_api-1.95.1/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-06 10:11:16.413450 windmill_api-1.95.1/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-06 10:11:16.433450 windmill_api-1.95.1/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-06 10:11:16.445450 windmill_api-1.95.1/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-06 10:11:16.461450 windmill_api-1.95.1/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-06 10:11:16.473450 windmill_api-1.95.1/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-06 10:11:16.485450 windmill_api-1.95.1/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-06 10:11:16.505450 windmill_api-1.95.1/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-06 10:11:16.509450 windmill_api-1.95.1/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-06 10:11:16.529450 windmill_api-1.95.1/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-06 10:11:16.537450 windmill_api-1.95.1/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-06 10:11:16.561450 windmill_api-1.95.1/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-06 10:11:16.581451 windmill_api-1.95.1/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-06 10:11:16.613451 windmill_api-1.95.1/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-06 10:11:16.609450 windmill_api-1.95.1/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-06 10:11:16.649451 windmill_api-1.95.1/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-06 10:11:16.649451 windmill_api-1.95.1/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-06 10:11:16.709451 windmill_api-1.95.1/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-06 10:11:16.705451 windmill_api-1.95.1/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-06 10:11:16.745451 windmill_api-1.95.1/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.737451 windmill_api-1.95.1/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-06 10:11:16.769451 windmill_api-1.95.1/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-06 10:11:16.769451 windmill_api-1.95.1/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-06 10:11:16.797451 windmill_api-1.95.1/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-06 10:11:16.801451 windmill_api-1.95.1/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-06 10:11:16.837451 windmill_api-1.95.1/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-06 10:11:16.841451 windmill_api-1.95.1/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.477417 windmill_api-1.95.1/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-06 10:11:16.881451 windmill_api-1.95.1/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.869451 windmill_api-1.95.1/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-06 10:11:16.913451 windmill_api-1.95.1/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-06 10:11:16.933451 windmill_api-1.95.1/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-06 10:11:16.969451 windmill_api-1.95.1/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-06 10:11:16.977451 windmill_api-1.95.1/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-06 10:11:17.009451 windmill_api-1.95.1/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.545417 windmill_api-1.95.1/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-06 10:11:17.013451 windmill_api-1.95.1/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-06 10:11:17.065451 windmill_api-1.95.1/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-06 10:11:02.469417 windmill_api-1.95.1/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-06 10:11:17.061452 windmill_api-1.95.1/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-06 10:11:17.093452 windmill_api-1.95.1/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.093452 windmill_api-1.95.1/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-06 10:11:17.125452 windmill_api-1.95.1/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-06 10:11:17.117452 windmill_api-1.95.1/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-06 10:11:17.149452 windmill_api-1.95.1/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-06 10:11:17.157452 windmill_api-1.95.1/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-06 10:11:17.177452 windmill_api-1.95.1/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.185452 windmill_api-1.95.1/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.205452 windmill_api-1.95.1/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-06 10:11:17.225452 windmill_api-1.95.1/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-06 10:11:17.241452 windmill_api-1.95.1/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-06 10:11:17.253452 windmill_api-1.95.1/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-06 10:11:17.277452 windmill_api-1.95.1/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-06 10:11:17.297452 windmill_api-1.95.1/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-06 10:11:17.325452 windmill_api-1.95.1/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-06 10:11:17.337452 windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-06 10:11:17.381452 windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-06 10:11:17.365452 windmill_api-1.95.1/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-06 10:11:17.409452 windmill_api-1.95.1/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-06 10:11:34.665474 windmill_api-1.95.1/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-06 10:11:17.433452 windmill_api-1.95.1/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-06 10:11:17.461452 windmill_api-1.95.1/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-05-06 10:11:11.853440 windmill_api-1.95.1/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-06 10:11:17.493452 windmill_api-1.95.1/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-06 10:11:17.525452 windmill_api-1.95.1/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-06 10:11:17.525452 windmill_api-1.95.1/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-06 10:11:17.577453 windmill_api-1.95.1/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-06 10:11:12.337441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-06 10:11:17.549453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-06 10:11:17.601453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-06 10:11:12.381441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-06 10:11:17.625453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-06 10:11:17.621453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-06 10:11:17.685453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-06 10:11:12.397441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-06 10:11:17.649453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-06 10:11:17.697453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-06 10:11:17.713453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-06 10:11:17.717453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-06 10:11:17.749453 windmill_api-1.95.1/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-06 10:11:17.813453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-06 10:11:17.773453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-06 10:11:12.605442 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-06 10:11:12.305441 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-06 10:11:17.797453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-06 10:11:17.869453 windmill_api-1.95.1/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-06 10:11:12.373441 windmill_api-1.95.1/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-06 10:11:12.265441 windmill_api-1.95.1/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-06 10:11:17.837453 windmill_api-1.95.1/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-06 10:11:17.885453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-06 10:11:17.933453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-06 10:11:12.281441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-06 10:11:17.909453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-06 10:11:17.937453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-06 10:11:17.961454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-06 10:11:17.977454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-06 10:11:12.437441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-06 10:11:17.993454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-06 10:11:18.033454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-06 10:11:12.381441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-06 10:11:18.017454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-06 10:11:11.705440 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-06 10:11:18.061454 windmill_api-1.95.1/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-06 10:11:18.069454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-06 10:11:18.145454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-06 10:11:18.109454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-06 10:11:18.141454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-06 10:11:18.173454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-06 10:11:18.181454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:12.353441 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-06 10:11:18.205454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-06 10:11:18.229454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-06 10:11:18.233454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-06 10:11:11.897440 windmill_api-1.95.1/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-06 10:11:18.273454 windmill_api-1.95.1/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-06 10:11:18.269454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-06 10:11:18.353454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-06 10:11:18.317454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-06 10:11:18.345454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-06 10:11:18.381455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-06 10:11:18.397455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:12.273441 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-06 10:11:18.413455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:11.837440 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-06 10:11:18.425454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-06 10:11:18.445455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-06 10:11:18.509455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-06 10:11:18.489455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-06 10:11:18.517455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-06 10:11:18.545455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-06 10:11:18.553455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-06 10:11:18.577455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-06 10:11:12.521442 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-06 10:11:18.585455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-06 10:11:18.605455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-06 10:11:12.361441 windmill_api-1.95.1/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-06 10:11:18.633455 windmill_api-1.95.1/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-06 10:11:18.625455 windmill_api-1.95.1/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-06 10:11:18.793455 windmill_api-1.95.1/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-06 10:11:18.653455 windmill_api-1.95.1/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-06 10:11:18.697455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-06 10:11:18.785455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-06 10:11:18.813455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-06 10:11:18.833455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-06 10:11:12.533442 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-06 10:11:18.841456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-06 10:11:18.873456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-06 10:11:11.821440 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-06 10:11:18.921456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-06 10:11:18.901455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-06 10:11:18.937456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-06 10:11:11.593439 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-06 10:11:18.949456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-06 10:11:18.973456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-06 10:11:12.605442 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-06 10:11:18.985456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-06 10:11:12.045441 windmill_api-1.95.1/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-06 10:11:11.581440 windmill_api-1.95.1/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-06 10:11:19.025456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-06 10:11:19.089456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-06 10:11:19.069456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-06 10:11:19.101456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-06 10:11:19.121456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-06 10:11:19.133456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:12.133441 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-06 10:11:19.149456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:12.129441 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-06 10:11:19.189456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-06 10:11:19.177456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-06 10:11:19.261456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-06 10:11:19.229456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-06 10:11:19.261456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-06 10:11:19.293456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-06 10:11:19.293456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-06 10:11:11.937440 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-06 10:11:19.321457 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-06 10:11:11.973440 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-06 10:11:19.325456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-06 10:11:19.349457 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-06 10:11:19.357457 windmill_api-1.95.1/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-06 10:11:19.389457 windmill_api-1.95.1/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-06 10:11:19.405457 windmill_api-1.95.1/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-06 10:11:19.417457 windmill_api-1.95.1/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-06 10:11:19.437457 windmill_api-1.95.1/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-06 10:11:19.457457 windmill_api-1.95.1/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-06 10:11:19.485457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:12.609442 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-06 10:11:19.485457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-06 10:11:19.509457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-06 10:11:19.541457 windmill_api-1.95.1/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-06 10:11:12.089441 windmill_api-1.95.1/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-06 10:11:19.537457 windmill_api-1.95.1/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-06 10:11:19.589457 windmill_api-1.95.1/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-06 10:11:19.569457 windmill_api-1.95.1/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-06 10:11:19.597457 windmill_api-1.95.1/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-06 10:11:19.613457 windmill_api-1.95.1/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-06 10:11:19.625457 windmill_api-1.95.1/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-06 10:11:19.637457 windmill_api-1.95.1/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-06 10:11:11.609439 windmill_api-1.95.1/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     2094 2023-05-06 10:11:19.661457 windmill_api-1.95.1/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-06 10:11:19.669457 windmill_api-1.95.1/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-06 10:11:19.697457 windmill_api-1.95.1/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-06 10:11:19.713457 windmill_api-1.95.1/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:19.717457 windmill_api-1.95.1/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-06 10:11:19.793458 windmill_api-1.95.1/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-06 10:11:12.609442 windmill_api-1.95.1/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:19.741458 windmill_api-1.95.1/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-06 10:11:19.781458 windmill_api-1.95.1/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-06 10:11:19.837458 windmill_api-1.95.1/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-06 10:11:19.841458 windmill_api-1.95.1/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-06 10:11:19.861458 windmill_api-1.95.1/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-06 10:11:19.881458 windmill_api-1.95.1/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-06 10:11:19.905458 windmill_api-1.95.1/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-06 10:11:19.913458 windmill_api-1.95.1/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-06 10:11:19.929458 windmill_api-1.95.1/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-06 10:11:19.937458 windmill_api-1.95.1/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-06 10:11:20.069458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-06 10:11:19.957458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-06 10:11:20.025458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-06 10:11:20.113458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-06 10:11:20.097458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-06 10:11:20.125458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-06 10:11:20.145458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-06 10:11:20.193458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-06 10:11:20.233459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-06 10:11:20.217459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-06 10:11:20.249459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-06 10:11:11.745440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-06 10:11:20.265459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-06 10:11:20.285459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-06 10:11:11.761440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-06 10:11:20.305459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-06 10:11:11.589439 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-06 10:11:12.105441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-06 10:11:20.333459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-06 10:11:20.425459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-06 10:11:20.373459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-06 10:11:20.405459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-06 10:11:20.441459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-06 10:11:20.457459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:11.773440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-06 10:11:20.469459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.345441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-06 10:11:20.489459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-06 10:11:20.501459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-06 10:11:20.577459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-06 10:11:20.541459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-06 10:11:20.601459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-06 10:11:20.613459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-06 10:11:20.633459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:12.329441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-06 10:11:20.645460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:12.149441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-06 10:11:20.661460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-06 10:11:20.677460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-06 10:11:20.689459 windmill_api-1.95.1/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-06 10:11:20.805460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-06 10:11:20.709460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-06 10:11:11.665440 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-06 10:11:20.733460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-06 10:11:20.777460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-06 10:11:20.841460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-06 10:11:11.757440 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-06 10:11:20.833460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-06 10:11:20.861460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-06 10:11:20.869460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-06 10:11:20.901460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-06 10:11:12.149441 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-06 10:11:20.893460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-06 10:11:20.933460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-06 10:11:12.073441 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-06 10:11:20.933460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-06 10:11:11.933440 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-06 10:11:20.957460 windmill_api-1.95.1/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-06 10:11:20.969460 windmill_api-1.95.1/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-06 10:11:21.009460 windmill_api-1.95.1/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-06 10:11:21.001460 windmill_api-1.95.1/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-06 10:11:21.025460 windmill_api-1.95.1/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-06 10:11:21.033460 windmill_api-1.95.1/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-06 10:11:21.065460 windmill_api-1.95.1/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-06 10:11:21.061460 windmill_api-1.95.1/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-06 10:11:21.093460 windmill_api-1.95.1/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-06 10:11:21.113460 windmill_api-1.95.1/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-06 10:11:21.113460 windmill_api-1.95.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-06 10:11:21.141461 windmill_api-1.95.1/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-06 10:11:21.141461 windmill_api-1.95.1/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-06 10:11:21.165461 windmill_api-1.95.1/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-06 10:11:21.245461 windmill_api-1.95.1/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-06 10:11:21.185461 windmill_api-1.95.1/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-06 10:11:21.237461 windmill_api-1.95.1/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-06 10:11:21.257461 windmill_api-1.95.1/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-06 10:11:21.333461 windmill_api-1.95.1/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-06 10:11:21.297461 windmill_api-1.95.1/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-06 10:11:21.329461 windmill_api-1.95.1/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-06 10:11:21.381461 windmill_api-1.95.1/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-06 10:11:21.361461 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-06 10:11:12.173441 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-06 10:11:21.393461 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-06 10:11:21.413461 windmill_api-1.95.1/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-06 10:11:21.425461 windmill_api-1.95.1/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-06 10:11:21.457461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.465461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.485461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.153441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.497461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-06 10:11:21.525461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.537461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.557461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.569461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-06 10:11:21.589461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.633462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.621461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.453441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.649462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.445441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-06 10:11:11.837440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-06 10:11:21.693462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-06 10:11:21.677462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-06 10:11:12.025441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-06 10:11:21.713462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-06 10:11:21.777462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-06 10:11:21.769462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-06 10:11:21.801462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-06 10:11:21.813462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-06 10:11:21.833462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:12.593442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-06 10:11:21.845462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:11.581440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-06 10:11:21.861462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-06 10:11:21.877462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-06 10:11:11.977440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-06 10:11:21.901462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-06 10:11:21.913462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-06 10:11:21.989462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-06 10:11:21.957462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-06 10:11:21.985462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-06 10:11:22.045462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.017462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:11.989440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-06 10:11:22.045462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:11.869440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-06 10:11:22.077463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-06 10:11:22.081462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-06 10:11:22.181463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-06 10:11:22.121463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-06 10:11:22.153463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-06 10:11:22.185463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-06 10:11:22.213463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:11.649440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-06 10:11:22.217463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-06 10:11:11.753440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-06 10:11:22.241463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-06 10:11:22.249463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:11.653440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-06 10:11:22.281463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-06 10:11:22.289463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-06 10:11:22.365463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-06 10:11:22.329463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-06 10:11:22.361463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-06 10:11:22.417463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.393463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:11.809440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-06 10:11:22.425463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:12.101441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-06 10:11:22.449463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-06 10:11:22.457463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:12.293441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-06 10:11:22.477464 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-06 10:11:12.469442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-06 10:11:22.501464 windmill_api-1.95.1/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-06 10:11:22.497464 windmill_api-1.95.1/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-06 10:11:22.541464 windmill_api-1.95.1/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-06 10:11:22.617464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-06 10:11:22.581464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-06 10:11:22.609464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.645464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-06 10:11:22.649464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:12.169441 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-06 10:11:22.669464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:11.701440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-06 10:11:22.681464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-06 10:11:22.697464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-06 10:11:22.765464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-06 10:11:22.741464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-06 10:11:22.769464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-06 10:11:22.797464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-06 10:11:22.825464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-06 10:11:11.789440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-06 10:11:22.833464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-06 10:11:11.713440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-06 10:11:22.857464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-06 10:11:22.861464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-06 10:11:22.877464 windmill_api-1.95.1/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-06 10:11:22.909464 windmill_api-1.95.1/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-06 10:11:22.961465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-06 10:11:22.969465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-06 10:11:22.993465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-06 10:11:11.761440 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-06 10:11:23.001465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-06 10:11:23.029465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-06 10:11:23.089465 windmill_api-1.95.1/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-06 10:11:23.053465 windmill_api-1.95.1/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-06 10:11:23.081465 windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-06 10:11:23.109465 windmill_api-1.95.1/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-06 10:11:23.125465 windmill_api-1.95.1/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-06 10:11:12.437441 windmill_api-1.95.1/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-06 10:11:23.233465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-06 10:11:23.149465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-06 10:11:23.181465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-06 10:11:12.085441 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-06 10:11:23.209465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-06 10:11:23.245465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-06 10:11:11.945440 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-06 10:11:23.269465 windmill_api-1.95.1/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-06 10:11:23.285465 windmill_api-1.95.1/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-06 10:11:23.353465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-06 10:11:23.357465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-06 10:11:23.385465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-06 10:11:23.393465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-06 10:11:23.417465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-06 10:11:23.421465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-06 10:11:12.329441 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-06 10:11:23.449465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-06 10:11:23.453465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-06 10:11:23.533465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-06 10:11:23.493465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-06 10:11:23.525465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-06 10:11:23.561465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-06 10:11:23.597465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-06 10:11:11.945440 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-06 10:11:23.593465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-06 10:11:12.129441 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-06 10:11:23.625465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-06 10:11:23.625465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-06 10:11:23.657465 windmill_api-1.95.1/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-06 10:11:23.645465 windmill_api-1.95.1/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-06 10:11:23.673465 windmill_api-1.95.1/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-06 10:11:23.709465 windmill_api-1.95.1/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-06 10:11:23.701465 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-06 10:11:12.293441 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-06 10:11:23.729465 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-06 10:11:12.173441 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-06 10:11:23.821465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-06 10:11:23.769465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-06 10:11:23.797465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-06 10:11:23.833465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-06 10:11:23.853465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-06 10:11:11.617440 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-06 10:11:23.861465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-06 10:11:12.533442 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-06 10:11:23.893465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-06 10:11:23.889465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-06 10:11:11.793440 windmill_api-1.95.1/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-06 10:11:23.941465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:12.557442 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-06 10:11:23.917465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-06 10:11:23.969465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-06 10:11:23.993465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-06 10:11:23.989465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-06 10:11:24.053465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-06 10:11:12.401441 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-06 10:11:24.013465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-06 10:11:24.061465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-06 10:11:11.997440 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-06 10:11:24.081465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-06 10:11:24.081465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-06 10:11:24.133465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-06 10:11:12.033440 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-06 10:11:24.109465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-06 10:11:24.193465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-06 10:11:12.333441 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-06 10:11:24.161465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-06 10:11:24.181465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-06 10:11:24.229465 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-06 10:11:12.181441 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-06 10:11:12.457441 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-06 10:11:24.221465 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-06 10:11:24.361466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-06 10:11:24.249465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-06 10:11:24.297465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-06 10:11:24.409465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-06 10:11:24.389465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-06 10:11:24.421465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-06 10:11:24.437466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-06 10:11:24.461465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-06 10:11:11.589439 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-06 10:11:24.521465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-06 10:11:24.489466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-06 10:11:24.517465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-06 10:11:12.069441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-06 10:11:24.545466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-06 10:11:24.561466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-06 10:11:24.625465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-06 10:11:11.861440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-06 10:11:12.009441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-06 10:11:24.605466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-06 10:11:24.689466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-06 10:11:24.669466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-06 10:11:24.697466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-06 10:11:24.761466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-06 10:11:24.729466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-06 10:11:11.865440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-06 10:11:24.761466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-06 10:11:12.481442 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-06 10:11:24.789466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-06 10:11:24.793465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-06 10:11:24.873466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-06 10:11:24.837466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-06 10:11:24.865465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-06 10:11:24.901466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-06 10:11:24.901466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:12.157441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-06 10:11:24.929466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:12.037440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-06 10:11:24.933466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-06 10:11:24.961466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-06 10:11:25.045466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-06 10:11:24.981466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-06 10:11:25.001466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-06 10:11:25.045466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-06 10:11:25.129466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-06 10:11:25.089466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-06 10:11:25.125466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-06 10:11:25.193466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-06 10:11:25.161466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-06 10:11:11.569440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-06 10:11:25.189466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-06 10:11:11.633440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-06 10:11:25.221466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-06 10:11:25.225466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-06 10:11:25.305466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-06 10:11:25.265466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-06 10:11:25.297466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-06 10:11:25.333466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-06 10:11:25.333466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-06 10:11:11.577439 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-06 10:11:25.369466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-06 10:11:25.365466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-06 10:11:25.425466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-06 10:11:25.401466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-06 10:11:25.473466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-06 10:11:25.445466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-06 10:11:25.465466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-06 10:11:25.509466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-06 10:11:25.597466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-06 10:11:25.553466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-06 10:11:25.581466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-06 10:11:25.617466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-06 10:11:25.629466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-06 10:11:11.785440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-06 10:11:25.645466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-06 10:11:11.881440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-06 10:11:25.661466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-06 10:11:25.673466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-06 10:11:25.745466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-06 10:11:25.713466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-06 10:11:25.745466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-06 10:11:25.777466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-06 10:11:25.777466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-06 10:11:11.741440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-06 10:11:25.805466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-06 10:11:25.809466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-06 10:11:25.837466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-06 10:11:25.849466 windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-06 10:11:25.857466 windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-06 10:11:25.881466 windmill_api-1.95.1/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-06 10:11:25.877466 windmill_api-1.95.1/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-06 10:11:25.913466 windmill_api-1.95.1/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-05-06 10:11:11.797440 windmill_api-1.95.1/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-06 10:11:25.905466 windmill_api-1.95.1/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-06 10:11:25.985466 windmill_api-1.95.1/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-06 10:11:25.933466 windmill_api-1.95.1/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-06 10:11:25.957466 windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-06 10:11:26.017466 windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-06 10:11:26.017466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-06 10:11:26.057466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-06 10:11:26.037466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-06 10:11:26.085466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-06 10:11:26.141466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-06 10:11:26.125466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-06 10:11:26.157466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-06 10:11:26.173466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-06 10:11:26.185466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:12.325441 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-06 10:11:26.205466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-06 10:11:26.217466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-06 10:11:26.233466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-06 10:11:26.301466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-06 10:11:26.277466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-06 10:11:26.305466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-06 10:11:26.337466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-06 10:11:26.337466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-06 10:11:12.617442 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-06 10:11:26.401466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-06 10:11:12.401441 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-06 10:11:26.405466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-06 10:11:26.433466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-06 10:11:26.445466 windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-06 10:11:12.561442 windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-06 10:11:26.473466 windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-06 10:11:26.461466 windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-06 10:11:11.941440 windmill_api-1.95.1/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-06 10:11:26.497466 windmill_api-1.95.1/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-06 10:11:26.513466 windmill_api-1.95.1/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-06 10:11:26.525466 windmill_api-1.95.1/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-06 10:11:26.569466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-06 10:11:26.545466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-06 10:11:26.605466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-06 10:11:12.005440 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-06 10:11:26.597466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-06 10:11:26.617466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-06 10:11:26.657466 windmill_api-1.95.1/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.641466 windmill_api-1.95.1/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-06 10:11:26.677466 windmill_api-1.95.1/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-06 10:11:26.685466 windmill_api-1.95.1/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-06 10:11:26.737466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:26.705466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.725466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-06 10:11:26.865466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-06 10:11:26.757466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-06 10:11:12.613442 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-06 10:11:12.097441 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.825466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-06 10:11:26.925466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-06 10:11:26.885466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-06 10:11:12.289441 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.909466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-06 10:11:26.993466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-06 10:11:27.001466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-06 10:11:11.897440 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-06 10:11:12.589442 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-06 10:11:27.017466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-06 10:11:11.705440 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-06 10:11:12.573442 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-06 10:11:27.025466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-06 10:11:27.049466 windmill_api-1.95.1/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-06 10:11:27.081466 windmill_api-1.95.1/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-06 10:11:27.081466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-06 10:11:27.109466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-06 10:11:27.113466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-06 10:11:11.641440 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-06 10:11:27.169466 windmill_api-1.95.1/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-06 10:11:27.133466 windmill_api-1.95.1/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-06 10:11:27.177466 windmill_api-1.95.1/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-06 10:11:27.245466 windmill_api-1.95.1/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-06 10:11:27.257466 windmill_api-1.95.1/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:11.741440 windmill_api-1.95.1/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-06 10:11:27.289466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-06 10:11:27.317466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-06 10:11:12.077441 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-06 10:11:27.317466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-06 10:11:27.341467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-06 10:11:27.345466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-06 10:11:27.381466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-06 10:11:11.593439 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-06 10:11:27.373467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-06 10:11:27.413467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-06 10:11:11.769440 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-06 10:11:27.409467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:11.989440 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-06 10:11:27.453467 windmill_api-1.95.1/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-06 10:11:27.433467 windmill_api-1.95.1/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-06 10:11:27.465467 windmill_api-1.95.1/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-06 10:11:27.493466 windmill_api-1.95.1/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-06 10:11:27.485467 windmill_api-1.95.1/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-06 10:11:27.517467 windmill_api-1.95.1/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-06 10:11:27.521467 windmill_api-1.95.1/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:12.461441 windmill_api-1.95.1/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-06 10:11:27.545467 windmill_api-1.95.1/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-06 10:11:27.545467 windmill_api-1.95.1/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-06 10:11:12.021440 windmill_api-1.95.1/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-06 10:11:27.581467 windmill_api-1.95.1/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-06 10:11:12.493441 windmill_api-1.95.1/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-06 10:11:27.597467 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:11.721440 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-06 10:11:27.641466 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-06 10:11:27.685467 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-06 10:11:12.565442 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-06 10:11:12.133441 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-06 10:11:27.669467 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-06 10:11:27.805467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-06 10:11:27.705467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-06 10:11:27.749467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-06 10:11:27.837467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-06 10:11:27.833467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-06 10:11:27.865467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-06 10:11:11.833440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-06 10:11:27.865467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-06 10:11:27.901467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-06 10:11:12.009441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-06 10:11:27.949467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-06 10:11:27.929467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-06 10:11:27.957467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-06 10:11:11.917440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-06 10:11:27.977467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-06 10:11:27.997467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-06 10:11:12.085441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-06 10:11:28.009467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-06 10:11:12.461441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:12.081441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-06 10:11:28.097467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-06 10:11:28.129467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-06 10:11:28.137467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-06 10:11:28.157467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-06 10:11:28.169467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-06 10:11:28.189467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-06 10:11:11.557439 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-06 10:11:28.201467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-06 10:11:12.201441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-06 10:11:28.221467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-06 10:11:28.229467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-06 10:11:28.305467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-06 10:11:28.269467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-06 10:11:28.297467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-06 10:11:28.333467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-06 10:11:28.337467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-06 10:11:11.577439 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-06 10:11:28.361467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-06 10:11:11.885440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-06 10:11:28.365467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-06 10:11:28.393467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-06 10:11:28.397467 windmill_api-1.95.1/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-06 10:11:28.421467 windmill_api-1.95.1/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-06 10:11:28.469467 windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-06 10:11:28.441467 windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-06 10:11:28.485467 windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-06 10:11:28.489467 windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-06 10:11:28.521467 windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-06 10:11:28.529467 windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-06 10:11:28.589467 windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-06 10:11:28.565467 windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-06 10:11:28.601467 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-06 10:11:28.629467 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-06 10:11:12.257441 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-06 10:11:28.641467 windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-06 10:11:28.649467 windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-06 10:11:12.109441 windmill_api-1.95.1/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-06 10:11:28.677467 windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-06 10:11:11.561439 windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-06 10:11:28.681467 windmill_api-1.95.1/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-06 10:11:28.877467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-06 10:11:28.705467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-06 10:11:28.749467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-06 10:11:28.833467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-06 10:11:28.861467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-06 10:11:28.893467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-06 10:11:12.621442 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-06 10:11:28.909467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-06 10:11:28.969467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-06 10:11:12.213441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-06 10:11:28.997467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-06 10:11:28.997467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-06 10:11:29.029467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-06 10:11:12.445441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-06 10:11:29.025467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-06 10:11:29.061467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-06 10:11:29.065467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-06 10:11:12.629442 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-06 10:11:12.105441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-06 10:11:29.105467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-06 10:11:29.149467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-06 10:11:29.145467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-06 10:11:29.177467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-06 10:11:29.185467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-06 10:11:29.205467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:12.309441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-06 10:11:29.213467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-06 10:11:29.237467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-06 10:11:29.297467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-06 10:11:29.357467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-06 10:11:29.337467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-06 10:11:29.365467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-06 10:11:29.389467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-06 10:11:29.397467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-06 10:11:12.109441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-06 10:11:29.421467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-06 10:11:11.849440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-06 10:11:29.429467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-06 10:11:29.449467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-05-06 10:11:29.497467 windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-06 10:11:29.469467 windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-06 10:11:29.505467 windmill_api-1.95.1/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-06 10:11:29.557467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-06 10:11:29.525467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-06 10:11:29.545467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-06 10:11:29.641467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-06 10:11:29.581467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-06 10:11:12.389441 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-06 10:11:12.385441 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-06 10:11:29.605467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-06 10:11:29.649467 windmill_api-1.95.1/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-06 10:11:29.673467 windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-06 10:11:29.677467 windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-06 10:11:29.713467 windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-06 10:11:12.405441 windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-06 10:11:29.789467 windmill_api-1.95.1/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-06 10:11:29.785467 windmill_api-1.95.1/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-06 10:11:29.849467 windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-06 10:11:29.809467 windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-06 10:11:29.849467 windmill_api-1.95.1/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-06 10:11:29.885467 windmill_api-1.95.1/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-06 10:11:29.885467 windmill_api-1.95.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-06 10:11:29.917467 windmill_api-1.95.1/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-06 10:11:29.929467 windmill_api-1.95.1/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-06 10:11:12.197441 windmill_api-1.95.1/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-06 10:11:29.941467 windmill_api-1.95.1/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-06 10:11:29.997467 windmill_api-1.95.1/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:29.961467 windmill_api-1.95.1/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-06 10:11:30.029467 windmill_api-1.95.1/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:30.013467 windmill_api-1.95.1/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-06 10:11:30.041467 windmill_api-1.95.1/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-06 10:11:30.057467 windmill_api-1.95.1/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-06 10:11:30.069467 windmill_api-1.95.1/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-06 10:11:30.097468 windmill_api-1.95.1/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-06 10:11:30.173467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-06 10:11:12.217441 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-06 10:11:30.125467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-06 10:11:30.149467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-06 10:11:30.229467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-06 10:11:30.209468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-06 10:11:11.685440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-06 10:11:30.237467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-06 10:11:30.265468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-06 10:11:11.721440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-06 10:11:30.261468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-06 10:11:11.685440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-06 10:11:30.305467 windmill_api-1.95.1/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-06 10:11:30.289467 windmill_api-1.95.1/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-06 10:11:30.361467 windmill_api-1.95.1/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-06 10:11:12.261441 windmill_api-1.95.1/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:12.413441 windmill_api-1.95.1/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-06 10:11:30.329467 windmill_api-1.95.1/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-06 10:11:30.413468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-06 10:11:30.433467 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-06 10:11:11.889440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-06 10:11:11.961440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-06 10:11:30.441468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-06 10:11:11.613440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-06 10:11:30.457468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-06 10:11:30.473467 windmill_api-1.95.1/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-06 10:11:30.497468 windmill_api-1.95.1/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-06 10:11:30.505468 windmill_api-1.95.1/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-06 10:11:30.537468 windmill_api-1.95.1/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-06 10:11:30.525468 windmill_api-1.95.1/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-06 10:11:30.613468 windmill_api-1.95.1/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-06 10:11:30.665468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-06 10:11:30.653468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-06 10:11:30.685468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-06 10:11:30.701468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-06 10:11:30.713468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-06 10:11:11.865440 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-06 10:11:30.729468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-06 10:11:12.477441 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-06 10:11:30.745468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-06 10:11:30.757468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-06 10:11:30.825469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-06 10:11:30.797469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-06 10:11:30.829469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-06 10:11:30.861469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-06 10:11:30.861469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-06 10:11:12.281441 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-06 10:11:30.889469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-06 10:11:11.701440 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-06 10:11:30.889469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-06 10:11:30.917469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-06 10:11:30.933469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-06 10:11:30.937469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-06 10:11:31.021469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-06 10:11:31.065469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-06 10:11:31.061469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-06 10:11:31.093469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-06 10:11:31.101469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-06 10:11:31.121469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-06 10:11:11.789440 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-06 10:11:31.129469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-06 10:11:11.757440 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-06 10:11:31.153469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-06 10:11:31.161470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-06 10:11:31.233470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-06 10:11:31.201470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-06 10:11:31.233470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-06 10:11:31.265470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-06 10:11:31.261470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-06 10:11:31.293470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-06 10:11:31.297470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-06 10:11:31.321470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-06 10:11:31.329470 windmill_api-1.95.1/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-06 10:11:31.357470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-06 10:11:31.357470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:11.825440 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-06 10:11:31.429470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:11.681440 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-06 10:11:31.397470 windmill_api-1.95.1/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-06 10:11:31.433470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-06 10:11:31.457470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-06 10:11:12.505442 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-06 10:11:31.465470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-06 10:11:12.121441 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-06 10:11:12.145441 windmill_api-1.95.1/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-06 10:11:31.509470 windmill_api-1.95.1/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-06 10:11:12.593442 windmill_api-1.95.1/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-06 10:11:31.489470 windmill_api-1.95.1/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-06 10:11:31.513470 windmill_api-1.95.1/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-06 10:11:31.545470 windmill_api-1.95.1/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-06 10:11:31.533470 windmill_api-1.95.1/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-06 10:11:12.433441 windmill_api-1.95.1/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-06 10:11:31.561470 windmill_api-1.95.1/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-06 10:11:31.589470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-06 10:11:31.625470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-06 10:11:11.689440 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-06 10:11:31.613470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-06 10:11:31.641470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-06 10:11:31.701470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-06 10:11:31.677470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-06 10:11:31.705470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-06 10:11:31.741470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-06 10:11:11.573439 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-06 10:11:31.733470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-06 10:11:12.525442 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-06 10:11:31.937471 windmill_api-1.95.1/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-06 10:11:31.761470 windmill_api-1.95.1/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-06 10:11:31.805470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-06 10:11:31.889470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-06 10:11:31.917471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-06 10:11:31.949471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-06 10:11:12.145441 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-06 10:11:31.965470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-06 10:11:31.985471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-06 10:11:32.049471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-06 10:11:32.013471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-06 10:11:32.041471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-06 10:11:11.769440 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-06 10:11:32.069471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-06 10:11:32.085471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-06 10:11:11.565440 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-06 10:11:32.157471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-06 10:11:12.417441 windmill_api-1.95.1/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:11.901440 windmill_api-1.95.1/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-06 10:11:32.129471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-06 10:11:32.277471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-06 10:11:32.201471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-06 10:11:32.229471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-06 10:11:32.265471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-06 10:11:32.297471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:12.269441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-06 10:11:32.305471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-06 10:11:12.201441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-06 10:11:32.325471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-06 10:11:32.333471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-06 10:11:32.409471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-06 10:11:32.373471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-06 10:11:32.405471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-06 10:11:32.437471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-06 10:11:32.437471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-06 10:11:32.465471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-06 10:11:12.097441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-06 10:11:32.469471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-06 10:11:32.497471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-06 10:11:32.513471 windmill_api-1.95.1/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-06 10:11:32.589471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-06 10:11:32.541471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-06 10:11:32.573471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-06 10:11:12.057441 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-06 10:11:12.521442 windmill_api-1.95.1/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-06 10:11:32.597471 windmill_api-1.95.1/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-06 10:11:32.613471 windmill_api-1.95.1/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-05-06 10:11:11.937440 windmill_api-1.95.1/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-06 10:11:32.625471 windmill_api-1.95.1/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-06 10:11:32.637471 windmill_api-1.95.1/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-06 10:11:32.677471 windmill_api-1.95.1/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-06 10:11:32.657471 windmill_api-1.95.1/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-06 10:11:32.693471 windmill_api-1.95.1/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-06 10:11:32.697471 windmill_api-1.95.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-06 10:11:32.717471 windmill_api-1.95.1/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-06 10:11:32.737471 windmill_api-1.95.1/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-06 10:11:32.745471 windmill_api-1.95.1/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-06 10:11:32.769472 windmill_api-1.95.1/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-06 10:11:32.765472 windmill_api-1.95.1/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-06 10:11:32.801472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-06 10:11:32.789471 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-06 10:11:32.897472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-06 10:11:32.885472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-06 10:11:32.925472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-06 10:11:32.925472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-06 10:11:32.961472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-06 10:11:32.957472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-06 10:11:11.729440 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-06 10:11:32.985472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-06 10:11:11.673440 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-06 10:11:32.989472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-06 10:11:33.017472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-06 10:11:33.145472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-06 10:11:33.057472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-06 10:11:33.089472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-06 10:11:33.121472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-06 10:11:33.153472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-06 10:11:12.465442 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-06 10:11:33.173472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-06 10:11:12.301441 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-06 10:11:33.181472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-06 10:11:33.205472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-06 10:11:33.205472 windmill_api-1.95.1/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-06 10:11:33.225472 windmill_api-1.95.1/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-06 10:11:33.241472 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-06 10:11:33.245472 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-06 10:11:12.385441 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-06 10:11:33.265472 windmill_api-1.95.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-06 10:11:33.265472 windmill_api-1.95.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-06 10:11:12.341441 windmill_api-1.95.1/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-06 10:11:33.325472 windmill_api-1.95.1/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-06 10:11:33.289472 windmill_api-1.95.1/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-06 10:11:33.309472 windmill_api-1.95.1/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-06 10:11:33.465472 windmill_api-1.95.1/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-06 10:11:33.345472 windmill_api-1.95.1/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-06 10:11:33.365472 windmill_api-1.95.1/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-06 10:11:12.269441 windmill_api-1.95.1/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-06 10:11:12.473441 windmill_api-1.95.1/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-06 10:11:33.389472 windmill_api-1.95.1/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-06 10:11:33.413472 windmill_api-1.95.1/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-06 10:11:33.437472 windmill_api-1.95.1/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-06 10:11:33.469472 windmill_api-1.95.1/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-06 10:11:33.489472 windmill_api-1.95.1/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-06 10:11:33.505472 windmill_api-1.95.1/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:12.397441 windmill_api-1.95.1/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-06 10:11:33.521472 windmill_api-1.95.1/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-06 10:11:12.181441 windmill_api-1.95.1/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-06 10:11:33.545472 windmill_api-1.95.1/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-06 10:11:33.565472 windmill_api-1.95.1/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-06 10:11:33.581472 windmill_api-1.95.1/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-06 10:11:33.613473 windmill_api-1.95.1/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-06 10:11:33.629473 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-06 10:11:33.637472 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-06 10:11:33.717473 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-06 10:11:33.681473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-06 10:11:33.701473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-06 10:11:33.745473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-06 10:11:33.801473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-06 10:11:33.793473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-06 10:11:33.825473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-06 10:11:33.833473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-06 10:11:33.909473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:12.369441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-06 10:11:33.861473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-06 10:11:33.893473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-06 10:11:33.925473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-06 10:11:33.993473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-06 10:11:33.969473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-06 10:11:33.997473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-06 10:11:34.029473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-06 10:11:34.029473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-06 10:11:12.093441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-06 10:11:34.057473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-06 10:11:12.273441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-06 10:11:34.057473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-06 10:11:34.085473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-06 10:11:34.093473 windmill_api-1.95.1/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-06 10:11:34.109473 windmill_api-1.95.1/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-06 10:11:34.121473 windmill_api-1.95.1/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-06 10:11:34.141473 windmill_api-1.95.1/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-06 10:11:34.153473 windmill_api-1.95.1/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-06 10:11:34.169473 windmill_api-1.95.1/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-06 10:11:34.181473 windmill_api-1.95.1/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-06 10:11:34.197473 windmill_api-1.95.1/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-06 10:11:34.201473 windmill_api-1.95.1/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-06 10:11:34.233473 windmill_api-1.95.1/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-06 10:11:34.237473 windmill_api-1.95.1/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-06 10:11:34.257473 windmill_api-1.95.1/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-06 10:11:34.301473 windmill_api-1.95.1/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-06 10:11:34.281473 windmill_api-1.95.1/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-06 10:11:34.313473 windmill_api-1.95.1/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-06 10:11:34.329473 windmill_api-1.95.1/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-06 10:11:34.449473 windmill_api-1.95.1/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-06 10:11:34.353473 windmill_api-1.95.1/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-06 10:11:34.473473 windmill_api-1.95.1/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-06 10:11:34.473473 windmill_api-1.95.1/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-06 10:11:34.513474 windmill_api-1.95.1/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-06 10:11:34.509473 windmill_api-1.95.1/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-06 10:11:34.537474 windmill_api-1.95.1/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-06 10:11:01.929416 windmill_api-1.95.1/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-06 10:11:34.529474 windmill_api-1.95.1/windmill_api/types.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.95.1/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.95.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-08 17:45:53.465227 windmill_api-1.96.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-08 17:45:53.473228 windmill_api-1.96.0/README.md
+-rw-r--r--   0        0        0      717 2023-05-08 17:45:53.465227 windmill_api-1.96.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-08 17:45:08.361165 windmill_api-1.96.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-08 17:45:09.081166 windmill_api-1.96.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.253166 windmill_api-1.96.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-08 17:45:22.989157 windmill_api-1.96.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-08 17:45:23.049157 windmill_api-1.96.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-08 17:45:23.041157 windmill_api-1.96.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-08 17:45:23.089157 windmill_api-1.96.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-08 17:45:23.125157 windmill_api-1.96.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-08 17:45:23.141157 windmill_api-1.96.0/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-08 17:45:23.181158 windmill_api-1.96.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-08 17:45:23.209158 windmill_api-1.96.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-08 17:45:23.261158 windmill_api-1.96.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-08 17:45:23.249158 windmill_api-1.96.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-08 17:45:23.369158 windmill_api-1.96.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-08 17:45:23.309158 windmill_api-1.96.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-08 17:45:23.361158 windmill_api-1.96.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.133165 windmill_api-1.96.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-08 17:45:23.417158 windmill_api-1.96.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-08 17:45:23.521159 windmill_api-1.96.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.341166 windmill_api-1.96.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-08 17:45:23.453159 windmill_api-1.96.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-08 17:45:23.501159 windmill_api-1.96.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-08 17:45:23.537159 windmill_api-1.96.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.265166 windmill_api-1.96.0/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-08 17:45:23.569159 windmill_api-1.96.0/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.345166 windmill_api-1.96.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-08 17:45:23.577159 windmill_api-1.96.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-08 17:45:23.613159 windmill_api-1.96.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.221166 windmill_api-1.96.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-08 17:45:23.621159 windmill_api-1.96.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-08 17:45:23.681159 windmill_api-1.96.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-08 17:45:23.661159 windmill_api-1.96.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-08 17:45:23.713160 windmill_api-1.96.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-08 17:45:23.737160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-08 17:45:23.785160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-08 17:45:23.825160 windmill_api-1.96.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-08 17:45:23.833160 windmill_api-1.96.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-08 17:45:23.869160 windmill_api-1.96.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-08 17:45:23.969160 windmill_api-1.96.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-08 17:45:23.917160 windmill_api-1.96.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-08 17:45:23.965160 windmill_api-1.96.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.329166 windmill_api-1.96.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-08 17:45:24.013161 windmill_api-1.96.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-08 17:45:24.009161 windmill_api-1.96.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-08 17:45:24.049161 windmill_api-1.96.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-08 17:45:24.073161 windmill_api-1.96.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-08 17:45:24.113161 windmill_api-1.96.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-08 17:45:24.145161 windmill_api-1.96.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-08 17:45:24.197161 windmill_api-1.96.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-08 17:45:24.217162 windmill_api-1.96.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-08 17:45:24.261162 windmill_api-1.96.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.337165 windmill_api-1.96.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-08 17:45:24.273162 windmill_api-1.96.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-08 17:45:24.321162 windmill_api-1.96.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-08 17:45:24.317162 windmill_api-1.96.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.321166 windmill_api-1.96.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-08 17:45:24.365162 windmill_api-1.96.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-08 17:45:24.361162 windmill_api-1.96.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-08 17:45:24.397162 windmill_api-1.96.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-08 17:45:24.425162 windmill_api-1.96.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-08 17:45:24.477162 windmill_api-1.96.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-08 17:45:24.509163 windmill_api-1.96.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-08 17:45:24.521163 windmill_api-1.96.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-08 17:45:24.553163 windmill_api-1.96.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.345166 windmill_api-1.96.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-08 17:45:24.581163 windmill_api-1.96.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-08 17:45:24.597163 windmill_api-1.96.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-08 17:45:24.693163 windmill_api-1.96.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-08 17:45:24.713163 windmill_api-1.96.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-08 17:45:24.753163 windmill_api-1.96.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.269166 windmill_api-1.96.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-08 17:45:24.761163 windmill_api-1.96.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-08 17:45:24.809163 windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 17:45:24.817164 windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-08 17:45:24.861164 windmill_api-1.96.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-08 17:45:24.877164 windmill_api-1.96.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-08 17:45:24.901164 windmill_api-1.96.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-08 17:45:24.933164 windmill_api-1.96.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:24.941164 windmill_api-1.96.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-08 17:45:24.985164 windmill_api-1.96.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-08 17:45:25.021164 windmill_api-1.96.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-08 17:45:25.057165 windmill_api-1.96.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-08 17:45:25.097164 windmill_api-1.96.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-08 17:45:25.277165 windmill_api-1.96.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-08 17:45:25.317165 windmill_api-1.96.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-08 17:45:25.485166 windmill_api-1.96.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-08 17:45:25.361166 windmill_api-1.96.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-08 17:45:25.405166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-08 17:45:25.461166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 17:45:25.517166 windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-08 17:45:25.565166 windmill_api-1.96.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-08 17:45:25.569166 windmill_api-1.96.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-08 17:45:25.673167 windmill_api-1.96.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-08 17:45:25.641167 windmill_api-1.96.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-08 17:45:25.717167 windmill_api-1.96.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-08 17:45:25.725167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-08 17:45:25.777167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-08 17:45:25.793167 windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.177166 windmill_api-1.96.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-08 17:45:25.833167 windmill_api-1.96.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-08 17:45:25.833167 windmill_api-1.96.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-08 17:45:25.877167 windmill_api-1.96.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-08 17:45:25.873167 windmill_api-1.96.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-08 17:45:25.913168 windmill_api-1.96.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-08 17:45:25.905167 windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-08 17:45:25.953168 windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-08 17:45:25.953168 windmill_api-1.96.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.305166 windmill_api-1.96.0/windmill_api/api/raw_app/__init__.py
+-rw-r--r--   0        0        0     2033 2023-05-08 17:45:25.997168 windmill_api-1.96.0/windmill_api/api/raw_app/create_raw_app.py
+-rw-r--r--   0        0        0     1781 2023-05-08 17:45:25.997168 windmill_api-1.96.0/windmill_api/api/raw_app/delete_raw_app.py
+-rw-r--r--   0        0        0     2786 2023-05-08 17:45:26.045168 windmill_api-1.96.0/windmill_api/api/raw_app/exists_raw_app.py
+-rw-r--r--   0        0        0     1979 2023-05-08 17:45:26.037168 windmill_api-1.96.0/windmill_api/api/raw_app/get_raw_app_data.py
+-rw-r--r--   0        0        0     7349 2023-05-08 17:45:26.177168 windmill_api-1.96.0/windmill_api/api/raw_app/list_raw_apps.py
+-rw-r--r--   0        0        0     2166 2023-05-08 17:45:26.089168 windmill_api-1.96.0/windmill_api/api/raw_app/update_raw_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.185166 windmill_api-1.96.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 17:45:26.129168 windmill_api-1.96.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-08 17:45:26.189169 windmill_api-1.96.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:26.217169 windmill_api-1.96.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-08 17:45:26.225169 windmill_api-1.96.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-08 17:45:26.273169 windmill_api-1.96.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-08 17:45:26.289169 windmill_api-1.96.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-08 17:45:26.333169 windmill_api-1.96.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-08 17:45:26.349169 windmill_api-1.96.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-08 17:45:26.377169 windmill_api-1.96.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-08 17:45:26.449169 windmill_api-1.96.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-08 17:45:26.437169 windmill_api-1.96.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-08 17:45:26.497170 windmill_api-1.96.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-08 17:45:26.489170 windmill_api-1.96.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-08 17:45:26.541170 windmill_api-1.96.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-08 17:45:26.545170 windmill_api-1.96.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.313166 windmill_api-1.96.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 17:45:26.581170 windmill_api-1.96.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:26.589170 windmill_api-1.96.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-08 17:45:26.649170 windmill_api-1.96.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-08 17:45:26.669170 windmill_api-1.96.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-08 17:45:26.761170 windmill_api-1.96.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-08 17:45:26.725170 windmill_api-1.96.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-08 17:45:26.777171 windmill_api-1.96.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-08 17:45:26.805171 windmill_api-1.96.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.201166 windmill_api-1.96.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-08 17:45:26.841171 windmill_api-1.96.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-08 17:45:26.845171 windmill_api-1.96.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 17:45:26.905171 windmill_api-1.96.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-08 17:45:26.889171 windmill_api-1.96.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-08 17:45:26.945171 windmill_api-1.96.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-08 17:45:26.969171 windmill_api-1.96.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 17:45:27.001171 windmill_api-1.96.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-08 17:45:27.025172 windmill_api-1.96.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-08 17:45:27.053172 windmill_api-1.96.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-08 17:45:27.065172 windmill_api-1.96.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-08 17:45:27.117172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-08 17:45:27.125172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-08 17:45:27.197172 windmill_api-1.96.0/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-08 17:45:27.201172 windmill_api-1.96.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-08 17:45:27.249172 windmill_api-1.96.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-08 17:45:27.253172 windmill_api-1.96.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-08 17:45:27.285173 windmill_api-1.96.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-08 17:45:27.445173 windmill_api-1.96.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-08 17:45:27.345173 windmill_api-1.96.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:27.381173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:27.425173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-08 17:45:27.473173 windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.101166 windmill_api-1.96.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-08 17:45:27.481173 windmill_api-1.96.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-08 17:45:27.513173 windmill_api-1.96.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.137166 windmill_api-1.96.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-08 17:45:27.541173 windmill_api-1.96.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-08 17:45:27.549173 windmill_api-1.96.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-08 17:45:27.577174 windmill_api-1.96.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-08 17:45:27.589174 windmill_api-1.96.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-08 17:45:27.617174 windmill_api-1.96.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-08 17:45:27.629174 windmill_api-1.96.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-08 17:45:27.653174 windmill_api-1.96.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-08 17:45:27.681174 windmill_api-1.96.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-08 17:45:27.713174 windmill_api-1.96.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-08 17:45:27.717174 windmill_api-1.96.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-08 17:45:27.753174 windmill_api-1.96.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-08 17:45:27.757174 windmill_api-1.96.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-08 17:45:27.797174 windmill_api-1.96.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-08 17:45:27.805174 windmill_api-1.96.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-08 17:45:27.833175 windmill_api-1.96.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-08 17:45:27.861175 windmill_api-1.96.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-08 17:45:27.889175 windmill_api-1.96.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-08 17:45:27.945175 windmill_api-1.96.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-08 17:45:27.973175 windmill_api-1.96.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-08 17:45:28.001175 windmill_api-1.96.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:28.013175 windmill_api-1.96.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-08 17:45:28.041175 windmill_api-1.96.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-08 17:45:28.053175 windmill_api-1.96.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-08 17:45:28.081175 windmill_api-1.96.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-08 17:45:28.101175 windmill_api-1.96.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-08 17:45:28.133175 windmill_api-1.96.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-08 17:45:28.157176 windmill_api-1.96.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.173166 windmill_api-1.96.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-08 17:45:28.193176 windmill_api-1.96.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-08 17:45:28.209176 windmill_api-1.96.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-08 17:45:28.249176 windmill_api-1.96.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-08 17:45:28.277176 windmill_api-1.96.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-08 17:45:28.305176 windmill_api-1.96.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-08 17:45:28.333176 windmill_api-1.96.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-08 17:45:28.357176 windmill_api-1.96.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.265166 windmill_api-1.96.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-08 17:45:28.381176 windmill_api-1.96.0/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-08 17:45:28.429176 windmill_api-1.96.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:45:09.157166 windmill_api-1.96.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-08 17:45:28.425176 windmill_api-1.96.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-08 17:45:28.457176 windmill_api-1.96.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.465176 windmill_api-1.96.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-08 17:45:28.497176 windmill_api-1.96.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-08 17:45:28.505176 windmill_api-1.96.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-08 17:45:28.549177 windmill_api-1.96.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-08 17:45:28.545176 windmill_api-1.96.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-08 17:45:28.589177 windmill_api-1.96.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.601177 windmill_api-1.96.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-08 17:45:28.649177 windmill_api-1.96.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-08 17:45:28.657177 windmill_api-1.96.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-08 17:45:28.705177 windmill_api-1.96.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-08 17:45:28.717177 windmill_api-1.96.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-08 17:45:28.757177 windmill_api-1.96.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-08 17:45:28.777177 windmill_api-1.96.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-08 17:45:28.805177 windmill_api-1.96.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-08 17:45:28.829177 windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-08 17:45:28.885177 windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-08 17:45:28.873177 windmill_api-1.96.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-08 17:45:28.917177 windmill_api-1.96.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-08 17:45:53.457228 windmill_api-1.96.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-08 17:45:28.953177 windmill_api-1.96.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-08 17:45:28.989177 windmill_api-1.96.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      325 2023-05-08 17:45:20.973151 windmill_api-1.96.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-08 17:45:29.025177 windmill_api-1.96.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-08 17:45:29.073177 windmill_api-1.96.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-08 17:45:29.109177 windmill_api-1.96.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-08 17:45:29.185178 windmill_api-1.96.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-08 17:45:21.713152 windmill_api-1.96.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-08 17:45:29.137178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-08 17:45:29.233178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-08 17:45:21.781153 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-08 17:45:29.229178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-08 17:45:29.261178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-08 17:45:29.309178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-08 17:45:29.289178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-08 17:45:29.365178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-08 17:45:21.145151 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-08 17:45:29.345178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-08 17:45:29.373178 windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-08 17:45:29.409178 windmill_api-1.96.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-08 17:45:29.509178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-08 17:45:29.433178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-08 17:45:22.105154 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-08 17:45:21.665152 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-08 17:45:29.481178 windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-08 17:45:29.569178 windmill_api-1.96.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-08 17:45:21.765153 windmill_api-1.96.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-08 17:45:21.601152 windmill_api-1.96.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-08 17:45:29.545178 windmill_api-1.96.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-08 17:45:29.601179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 17:45:29.665179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 17:45:21.625152 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 17:45:29.633179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 17:45:29.669179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 17:45:29.741179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 17:45:29.749179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 17:45:21.861153 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 17:45:29.785179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 17:45:29.813179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 17:45:21.781153 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 17:45:29.821179 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 17:45:20.753150 windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 17:45:29.865179 windmill_api-1.96.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-08 17:45:29.869179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 17:45:29.985179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 17:45:29.921179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 17:45:29.961179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 17:45:30.009179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 17:45:30.029179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:21.737152 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 17:45:30.053179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:21.165151 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 17:45:30.077179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 17:45:30.093179 windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 17:45:21.045151 windmill_api-1.96.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-08 17:45:30.133180 windmill_api-1.96.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-08 17:45:30.141179 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 17:45:30.289180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 17:45:30.205180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 17:45:30.261180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 17:45:30.305180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 17:45:30.333180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:21.609152 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 17:45:30.345180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:20.949151 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 17:45:30.381180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 17:45:30.389180 windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 17:45:30.513180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 17:45:30.445180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 17:45:30.489180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 17:45:30.537180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 17:45:30.557180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 17:45:30.581180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 17:45:21.973153 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 17:45:30.609180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 17:45:30.629180 windmill_api-1.96.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 17:45:21.749153 windmill_api-1.96.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-08 17:45:30.657180 windmill_api-1.96.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 17:45:30.657180 windmill_api-1.96.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-08 17:45:30.897181 windmill_api-1.96.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-08 17:45:30.689180 windmill_api-1.96.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 17:45:30.749181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-08 17:45:30.889181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-08 17:45:30.929181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-08 17:45:30.945181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-08 17:45:21.997153 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-08 17:45:30.969181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-08 17:45:31.005181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-08 17:45:20.921151 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-08 17:45:31.121181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-08 17:45:31.041181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 17:45:31.093181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-08 17:45:20.593150 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-08 17:45:31.137181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-08 17:45:31.169181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-08 17:45:22.105154 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-08 17:45:31.193181 windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-08 17:45:21.281151 windmill_api-1.96.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-08 17:45:20.577150 windmill_api-1.96.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-08 17:45:31.237182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-08 17:45:31.313182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-08 17:45:31.293182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 17:45:31.357182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 17:45:31.365182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 17:45:31.393182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:21.413152 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 17:45:31.405182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:21.405151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 17:45:31.433182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 17:45:31.469182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-08 17:45:31.537182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-08 17:45:31.521182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-08 17:45:31.561182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-08 17:45:31.577182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-08 17:45:31.601182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-08 17:45:21.117151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-08 17:45:31.609182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-08 17:45:21.173151 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-08 17:45:31.641182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-08 17:45:31.649182 windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-08 17:45:31.681182 windmill_api-1.96.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-08 17:45:31.697182 windmill_api-1.96.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-08 17:45:31.717182 windmill_api-1.96.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-08 17:45:31.737182 windmill_api-1.96.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-08 17:45:31.769183 windmill_api-1.96.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-08 17:45:31.785183 windmill_api-1.96.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 17:45:31.833183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:22.117154 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 17:45:31.837183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 17:45:31.861183 windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-08 17:45:31.881183 windmill_api-1.96.0/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-08 17:45:21.341151 windmill_api-1.96.0/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-08 17:45:31.901183 windmill_api-1.96.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-08 17:45:31.925183 windmill_api-1.96.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-08 17:45:31.941183 windmill_api-1.96.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-08 17:45:31.965183 windmill_api-1.96.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-08 17:45:31.997183 windmill_api-1.96.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-08 17:45:31.997183 windmill_api-1.96.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-08 17:45:32.029183 windmill_api-1.96.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-08 17:45:20.617150 windmill_api-1.96.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     1732 2023-05-08 17:45:32.037183 windmill_api-1.96.0/windmill_api/models/create_raw_app_json_body.py
+-rw-r--r--   0        0        0     2094 2023-05-08 17:45:32.073183 windmill_api-1.96.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-08 17:45:32.081183 windmill_api-1.96.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-08 17:45:32.125183 windmill_api-1.96.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-08 17:45:32.137183 windmill_api-1.96.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:32.149183 windmill_api-1.96.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-08 17:45:32.237183 windmill_api-1.96.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-08 17:45:22.113154 windmill_api-1.96.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-08 17:45:20.581150 windmill_api-1.96.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:32.189183 windmill_api-1.96.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-08 17:45:32.241183 windmill_api-1.96.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-08 17:45:32.281183 windmill_api-1.96.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-08 17:45:32.297183 windmill_api-1.96.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-08 17:45:32.341184 windmill_api-1.96.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-08 17:45:32.349184 windmill_api-1.96.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-08 17:45:32.389184 windmill_api-1.96.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-08 17:45:32.385184 windmill_api-1.96.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-08 17:45:32.437184 windmill_api-1.96.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-08 17:45:32.425184 windmill_api-1.96.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-08 17:45:32.621184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-08 17:45:32.465184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-08 17:45:32.557184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-08 17:45:32.689184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-08 17:45:32.657184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-08 17:45:32.701184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-08 17:45:32.733184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-08 17:45:32.753184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-08 17:45:32.865184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-08 17:45:32.789184 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-08 17:45:32.873185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-08 17:45:20.809150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-08 17:45:32.913185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-08 17:45:32.921185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-08 17:45:20.833150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-08 17:45:32.969185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-08 17:45:20.589150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 17:45:21.365152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-08 17:45:32.989185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-08 17:45:33.129185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-08 17:45:33.041185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-08 17:45:33.089185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-08 17:45:33.133185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-08 17:45:33.173185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:20.849150 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 17:45:33.177185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.725152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-08 17:45:33.213185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-08 17:45:33.221185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-08 17:45:33.337185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-08 17:45:33.285185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-08 17:45:33.325185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-08 17:45:33.377185 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-08 17:45:33.385186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.705152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-08 17:45:33.445186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.433152 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-08 17:45:33.433186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-08 17:45:33.473186 windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-08 17:45:33.501186 windmill_api-1.96.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-08 17:45:33.613186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-08 17:45:33.529186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 17:45:20.697150 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-08 17:45:33.565186 windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-08 17:45:33.625186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 17:45:33.733186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 17:45:20.829150 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 17:45:33.661186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 17:45:33.701186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 17:45:33.741186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 17:45:33.785186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 17:45:21.433152 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 17:45:33.781186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 17:45:33.841186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 17:45:21.321151 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 17:45:33.825186 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 17:45:21.105151 windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-08 17:45:33.865186 windmill_api-1.96.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-08 17:45:33.901186 windmill_api-1.96.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-08 17:45:33.921187 windmill_api-1.96.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-08 17:45:33.953187 windmill_api-1.96.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-08 17:45:33.953187 windmill_api-1.96.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-08 17:45:33.989187 windmill_api-1.96.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-08 17:45:34.017187 windmill_api-1.96.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-08 17:45:34.033187 windmill_api-1.96.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-08 17:45:34.061187 windmill_api-1.96.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-08 17:45:34.105187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-08 17:45:34.089187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-08 17:45:34.133187 windmill_api-1.96.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-08 17:45:34.145187 windmill_api-1.96.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-08 17:45:34.161187 windmill_api-1.96.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-08 17:45:34.281187 windmill_api-1.96.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 17:45:34.197187 windmill_api-1.96.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-08 17:45:34.269187 windmill_api-1.96.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-08 17:45:34.297187 windmill_api-1.96.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-08 17:45:34.409187 windmill_api-1.96.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-08 17:45:34.349187 windmill_api-1.96.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-08 17:45:34.393187 windmill_api-1.96.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-08 17:45:34.437188 windmill_api-1.96.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-08 17:45:34.453188 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-08 17:45:21.469152 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-08 17:45:34.477187 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-08 17:45:21.013151 windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-08 17:45:34.501188 windmill_api-1.96.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-08 17:45:34.541188 windmill_api-1.96.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-08 17:45:34.561188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.589188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.609188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.441151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.633188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-08 17:45:21.157151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-08 17:45:34.661188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.689188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.705188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:22.073154 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.737188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.821153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-08 17:45:20.957151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-08 17:45:34.749188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-08 17:45:34.789188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 17:45:34.837188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.885153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 17:45:34.833188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.873153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-08 17:45:20.945150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-08 17:45:34.913188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-08 17:45:34.881188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 17:45:21.253151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-08 17:45:34.929188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-08 17:45:35.029188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 17:45:34.985188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 17:45:35.029188 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 17:45:35.101189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 17:45:35.073189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:22.085154 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 17:45:35.113189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:20.577150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 17:45:35.149189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 17:45:35.161189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-08 17:45:21.173151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-08 17:45:35.205189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-08 17:45:35.225189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 17:45:35.325189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 17:45:35.281189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 17:45:35.321189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 17:45:35.405189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 17:45:35.369189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.201151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 17:45:35.413189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:20.997151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 17:45:35.449189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 17:45:35.457189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-08 17:45:35.569190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 17:45:35.517189 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 17:45:35.557190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 17:45:35.633190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 17:45:35.609190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:20.677150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 17:45:35.653190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 17:45:20.821150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 17:45:35.677190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 17:45:35.697190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:20.685150 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-08 17:45:35.737190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-08 17:45:35.749190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 17:45:35.861190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 17:45:35.805190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 17:45:35.849190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 17:45:35.893190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 17:45:35.905190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:20.905151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 17:45:35.973190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.361151 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 17:45:35.949190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 17:45:35.993190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:21.645152 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-08 17:45:36.013190 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-08 17:45:21.905153 windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-08 17:45:36.037190 windmill_api-1.96.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-08 17:45:36.045190 windmill_api-1.96.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-08 17:45:36.097190 windmill_api-1.96.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-08 17:45:36.161191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-08 17:45:36.257191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-08 17:45:36.205191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-08 17:45:36.257191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-08 17:45:36.301191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:21.465152 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-08 17:45:36.293191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:20.749150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-08 17:45:36.333191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-08 17:45:36.353191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-08 17:45:36.449191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-08 17:45:36.413191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-08 17:45:36.457191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-08 17:45:36.497191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-08 17:45:36.541191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 17:45:20.877150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-08 17:45:36.537191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 17:45:20.765150 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-08 17:45:36.581191 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-08 17:45:36.589192 windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-08 17:45:36.609192 windmill_api-1.96.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-08 17:45:36.657192 windmill_api-1.96.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-08 17:45:36.729192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-08 17:45:36.693192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-08 17:45:36.733192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-08 17:45:20.837150 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-08 17:45:36.769192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-08 17:45:36.813192 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-08 17:45:36.905192 windmill_api-1.96.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-08 17:45:36.853192 windmill_api-1.96.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-08 17:45:36.897192 windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-08 17:45:21.825153 windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-08 17:45:36.949192 windmill_api-1.96.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-08 17:45:36.961192 windmill_api-1.96.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-08 17:45:21.861153 windmill_api-1.96.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-08 17:45:37.073192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-08 17:45:36.997192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-08 17:45:37.101192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-08 17:45:21.341151 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-08 17:45:37.113192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-08 17:45:37.153192 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-08 17:45:21.129151 windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-08 17:45:37.165192 windmill_api-1.96.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-08 17:45:37.213193 windmill_api-1.96.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-08 17:45:37.277193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-08 17:45:37.269193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 17:45:37.313193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 17:45:37.365193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 17:45:37.357193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 17:45:37.397193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:45:21.697152 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 17:45:37.413193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 17:45:37.437193 windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 17:45:37.529193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 17:45:37.493193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 17:45:37.533193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 17:45:37.585193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 17:45:37.573193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 17:45:21.125151 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 17:45:37.653193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 17:45:21.405151 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 17:45:37.625193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 17:45:37.669193 windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-08 17:45:37.697193 windmill_api-1.96.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-08 17:45:37.697193 windmill_api-1.96.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-08 17:45:37.729194 windmill_api-1.96.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-08 17:45:37.769194 windmill_api-1.96.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-08 17:45:37.769194 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-08 17:45:21.645152 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-08 17:45:37.809194 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-08 17:45:21.469152 windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-08 17:45:37.929194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-08 17:45:37.865194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 17:45:37.905194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 17:45:37.953194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 17:45:37.969194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:45:20.625150 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 17:45:37.989194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:45:21.997153 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 17:45:38.017194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 17:45:38.029194 windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-08 17:45:20.881150 windmill_api-1.96.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-08 17:45:38.093194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:22.029153 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-08 17:45:38.061194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-08 17:45:38.129194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-08 17:45:21.165151 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-08 17:45:38.137194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-08 17:45:38.189194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-08 17:45:38.225195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-08 17:45:21.809153 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-08 17:45:38.221194 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-08 17:45:38.293195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-08 17:45:21.209151 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-08 17:45:38.261195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-08 17:45:38.293195 windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-08 17:45:38.361195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-08 17:45:21.265151 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-08 17:45:38.329195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-08 17:45:38.401195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-08 17:45:21.705152 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-08 17:45:38.397195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-08 17:45:38.425195 windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-08 17:45:38.509195 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-08 17:45:21.485152 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-08 17:45:21.889153 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-08 17:45:38.465195 windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-08 17:45:38.661195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-08 17:45:38.545195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-08 17:45:38.609195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-08 17:45:38.729195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-08 17:45:38.729195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-08 17:45:38.769195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-08 17:45:20.961151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 17:45:38.769195 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-08 17:45:38.813196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-08 17:45:38.885196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-08 17:45:38.845196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 17:45:38.893196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 17:45:21.317151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 17:45:38.929196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 17:45:38.941196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 17:45:20.961151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-08 17:45:38.985196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-08 17:45:20.989151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 17:45:21.229151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-08 17:45:39.013196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-08 17:45:39.145196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-08 17:45:39.073196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-08 17:45:39.117196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-08 17:45:39.165196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-08 17:45:39.189196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-08 17:45:20.997151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-08 17:45:39.217196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-08 17:45:21.921153 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-08 17:45:39.229196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-08 17:45:39.301196 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-08 17:45:39.345197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-08 17:45:39.365197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 17:45:39.393197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 17:45:39.417197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 17:45:39.433197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.445152 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 17:45:39.461197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.265151 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 17:45:39.477197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 17:45:39.505197 windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-08 17:45:39.625197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-08 17:45:39.533197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-08 17:45:39.565197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-08 17:45:39.625197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-08 17:45:39.741197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-08 17:45:39.681197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 17:45:39.725197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 17:45:39.777197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 17:45:39.785197 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 17:45:20.553150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 17:45:39.821198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 17:45:20.649150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 17:45:39.873198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 17:45:39.861198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-08 17:45:39.981198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-08 17:45:39.933198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-08 17:45:39.973198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-08 17:45:40.017198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-08 17:45:40.021198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 17:45:20.569150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-08 17:45:40.061198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-08 17:45:40.065198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-08 17:45:40.105198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-08 17:45:40.177198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-08 17:45:40.225198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-08 17:45:40.209198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-08 17:45:40.241198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-08 17:45:40.285198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-08 17:45:40.365198 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-08 17:45:40.341199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-08 17:45:40.381199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-08 17:45:40.409199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-08 17:45:40.457199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-08 17:45:20.869150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-08 17:45:40.449199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-08 17:45:21.021151 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-08 17:45:40.485199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-08 17:45:40.493199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-08 17:45:40.597199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-08 17:45:40.545199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-08 17:45:40.589199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-08 17:45:40.637199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-08 17:45:40.637199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-08 17:45:20.805150 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-08 17:45:40.709199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-08 17:45:22.065154 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-08 17:45:40.677199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-08 17:45:40.721199 windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-08 17:45:40.757199 windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-08 17:45:40.745199 windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-08 17:45:40.789199 windmill_api-1.96.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-08 17:45:40.785199 windmill_api-1.96.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-08 17:45:40.829199 windmill_api-1.96.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      325 2023-05-08 17:45:20.885151 windmill_api-1.96.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-08 17:45:40.817199 windmill_api-1.96.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-08 17:45:40.881199 windmill_api-1.96.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-08 17:45:40.853199 windmill_api-1.96.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-08 17:45:40.889200 windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-08 17:45:40.913200 windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-08 17:45:40.925200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-08 17:45:41.005200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-08 17:45:40.957200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-08 17:45:41.013200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-08 17:45:41.117200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-08 17:45:41.073200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-08 17:45:41.117200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-08 17:45:41.157200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-08 17:45:41.153200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.697152 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-08 17:45:41.197200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:20.957151 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-08 17:45:41.197200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-08 17:45:41.237200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-08 17:45:41.357200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-08 17:45:41.297200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-08 17:45:41.341200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-08 17:45:41.389201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-08 17:45:41.401200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-08 17:45:22.125154 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-08 17:45:41.433200 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 17:45:41.445201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-08 17:45:41.521201 windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-08 17:45:41.497201 windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-08 17:45:22.041154 windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-08 17:45:41.553201 windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-08 17:45:41.553201 windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-08 17:45:21.117151 windmill_api-1.96.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-08 17:45:41.597201 windmill_api-1.96.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-08 17:45:41.609201 windmill_api-1.96.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-08 17:45:41.637201 windmill_api-1.96.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-08 17:45:41.677201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-08 17:45:41.661201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-08 17:45:41.725201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-08 17:45:21.221151 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-08 17:45:41.713201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-08 17:45:41.741201 windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-08 17:45:41.833201 windmill_api-1.96.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.765201 windmill_api-1.96.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-08 17:45:41.817201 windmill_api-1.96.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-08 17:45:41.857201 windmill_api-1.96.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-08 17:45:41.913201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:41.889201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.917201 windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-08 17:45:42.029202 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 17:45:41.945201 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 17:45:22.117154 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 17:45:21.357151 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 17:45:41.973202 windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-08 17:45:42.141202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 17:45:42.057202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 17:45:21.641152 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 17:45:21.377151 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 17:45:42.093202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-08 17:45:42.197202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-08 17:45:42.241202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-08 17:45:21.049151 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-08 17:45:22.081154 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-08 17:45:42.229202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-08 17:45:20.757150 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-08 17:45:22.061154 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-08 17:45:42.265202 windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-08 17:45:42.281202 windmill_api-1.96.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-08 17:45:42.385202 windmill_api-1.96.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-08 17:45:42.321202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-08 17:45:42.357202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-08 17:45:42.397202 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-08 17:45:20.661150 windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-08 17:45:42.501202 windmill_api-1.96.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 17:45:42.425202 windmill_api-1.96.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-08 17:45:42.485202 windmill_api-1.96.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-08 17:45:42.521203 windmill_api-1.96.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-08 17:45:42.557203 windmill_api-1.96.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-08 17:45:20.809150 windmill_api-1.96.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-08 17:45:42.657203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-08 17:45:42.649203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-08 17:45:21.329151 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-08 17:45:42.689203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-08 17:45:42.693203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-08 17:45:42.733203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-08 17:45:42.749203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-08 17:45:20.597150 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-08 17:45:42.769203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-08 17:45:42.801203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-08 17:45:20.849150 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 17:45:42.809203 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:21.193151 windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-08 17:45:42.857203 windmill_api-1.96.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-08 17:45:42.833203 windmill_api-1.96.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-08 17:45:42.869203 windmill_api-1.96.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-08 17:45:21.013151 windmill_api-1.96.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 17:45:42.913203 windmill_api-1.96.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-08 17:45:42.957203 windmill_api-1.96.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-08 17:45:42.953203 windmill_api-1.96.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-08 17:45:42.997203 windmill_api-1.96.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:21.893153 windmill_api-1.96.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 17:45:43.001203 windmill_api-1.96.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-08 17:45:43.033203 windmill_api-1.96.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-08 17:45:21.249151 windmill_api-1.96.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-08 17:45:43.053204 windmill_api-1.96.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-08 17:45:21.937153 windmill_api-1.96.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-08 17:45:43.105204 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:20.773150 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-08 17:45:43.085204 windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-08 17:45:21.453152 windmill_api-1.96.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-08 17:45:43.161204 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-08 17:45:22.041154 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-08 17:45:21.413152 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-08 17:45:43.145204 windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-08 17:45:43.341204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-08 17:45:43.189204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-08 17:45:43.289204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-08 17:45:43.405204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-08 17:45:43.381204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-08 17:45:43.421204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-08 17:45:20.941151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-08 17:45:43.445204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-08 17:45:43.533204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-08 17:45:21.229151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-08 17:45:43.565204 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-08 17:45:43.569205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-08 17:45:43.605205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-08 17:45:21.081151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-08 17:45:43.609205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-08 17:45:43.657205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-08 17:45:21.337151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-08 17:45:43.661205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-08 17:45:21.893153 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:21.333151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-08 17:45:43.725205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-08 17:45:43.853205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-08 17:45:43.785205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-08 17:45:43.825205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-08 17:45:43.873205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-08 17:45:43.893205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-08 17:45:20.537150 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-08 17:45:43.917205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-08 17:45:21.517152 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 17:45:43.937205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-08 17:45:43.961205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-08 17:45:44.061205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-08 17:45:44.021206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-08 17:45:44.065205 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-08 17:45:44.109206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-08 17:45:44.181206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-08 17:45:20.569150 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-08 17:45:44.153206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-08 17:45:21.025151 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-08 17:45:44.193206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-08 17:45:44.229206 windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-08 17:45:44.237206 windmill_api-1.96.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-08 17:45:44.269206 windmill_api-1.96.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-08 17:45:44.281206 windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 17:45:44.301206 windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-08 17:45:44.429206 windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-08 17:45:44.333206 windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-08 17:45:44.385206 windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-08 17:45:44.437206 windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 17:45:44.477206 windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-08 17:45:44.493206 windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 17:45:44.525206 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-08 17:45:44.557206 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-08 17:45:21.589152 windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-08 17:45:44.581206 windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-08 17:45:44.585206 windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-08 17:45:21.377151 windmill_api-1.96.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 17:45:44.629207 windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-08 17:45:20.541150 windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-08 17:45:44.633206 windmill_api-1.96.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-08 17:45:44.933207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-08 17:45:44.669207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-08 17:45:44.733207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-08 17:45:44.861207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-08 17:45:44.897207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 17:45:45.005207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 17:45:22.133154 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 17:45:44.973207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 17:45:45.029207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 17:45:21.537152 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-08 17:45:45.125208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-08 17:45:45.065207 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-08 17:45:45.105208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-08 17:45:21.869153 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-08 17:45:45.145208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-08 17:45:45.173208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-08 17:45:21.161151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-08 17:45:45.193208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-08 17:45:22.145154 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-08 17:45:21.369151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-08 17:45:45.237208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-08 17:45:45.381208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-08 17:45:45.297208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 17:45:45.341208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 17:45:45.389208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 17:45:45.421208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.673152 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 17:45:45.429208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.149151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 17:45:45.465208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 17:45:45.469208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-08 17:45:45.585208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-08 17:45:45.601208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 17:45:45.621209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 17:45:45.649208 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 17:45:45.673209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 17:45:21.373151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 17:45:45.693209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 17:45:20.969151 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 17:45:45.713209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 17:45:45.737209 windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3045 2023-05-08 17:45:45.777209 windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item.py
+-rw-r--r--   0        0        0     1294 2023-05-08 17:45:45.761209 windmill_api-1.96.0/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     4884 2023-05-08 17:45:45.865209 windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 17:45:45.801209 windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-08 17:45:45.853209 windmill_api-1.96.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-08 17:45:46.029209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-08 17:45:45.897209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-08 17:45:45.925209 windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-08 17:45:46.057210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 17:45:46.061210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 17:45:21.793153 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 17:45:21.785153 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-08 17:45:46.153210 windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-08 17:45:46.125210 windmill_api-1.96.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-08 17:45:46.169210 windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-08 17:45:46.193210 windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-08 17:45:46.225210 windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-08 17:45:21.817153 windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-08 17:45:46.285210 windmill_api-1.96.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-08 17:45:46.261210 windmill_api-1.96.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-08 17:45:46.357210 windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 17:45:46.317210 windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-08 17:45:46.369210 windmill_api-1.96.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 17:45:46.401210 windmill_api-1.96.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-08 17:45:46.417210 windmill_api-1.96.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-08 17:45:46.449211 windmill_api-1.96.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-08 17:45:46.485211 windmill_api-1.96.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-08 17:45:21.509152 windmill_api-1.96.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-08 17:45:46.481211 windmill_api-1.96.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     2913 2023-05-08 17:45:46.537211 windmill_api-1.96.0/windmill_api/models/listable_raw_app.py
+-rw-r--r--   0        0        0     1225 2023-05-08 17:45:46.513211 windmill_api-1.96.0/windmill_api/models/listable_raw_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-08 17:45:46.605211 windmill_api-1.96.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:46.565211 windmill_api-1.96.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-08 17:45:46.749211 windmill_api-1.96.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:46.633211 windmill_api-1.96.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-08 17:45:46.737211 windmill_api-1.96.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-08 17:45:46.777211 windmill_api-1.96.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-08 17:45:46.797211 windmill_api-1.96.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-08 17:45:46.837211 windmill_api-1.96.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-08 17:45:46.893211 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-08 17:45:21.545152 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-08 17:45:46.881212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-08 17:45:46.917212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-08 17:45:46.933212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-08 17:45:46.985212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-08 17:45:20.725150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 17:45:46.969212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-08 17:45:47.025212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-08 17:45:20.777150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-08 17:45:47.021212 windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 17:45:20.729150 windmill_api-1.96.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-08 17:45:47.081212 windmill_api-1.96.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-08 17:45:47.057212 windmill_api-1.96.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-08 17:45:47.165212 windmill_api-1.96.0/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-08 17:45:21.593152 windmill_api-1.96.0/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.829153 windmill_api-1.96.0/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-08 17:45:47.117212 windmill_api-1.96.0/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-08 17:45:47.241212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-08 17:45:47.345213 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-08 17:45:21.033151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-08 17:45:21.153151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-08 17:45:47.277212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-08 17:45:20.621150 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-08 17:45:21.145151 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-08 17:45:47.313212 windmill_api-1.96.0/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-08 17:45:47.369213 windmill_api-1.96.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-08 17:45:47.401213 windmill_api-1.96.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-08 17:45:47.413213 windmill_api-1.96.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-08 17:45:47.465213 windmill_api-1.96.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 17:45:47.441213 windmill_api-1.96.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-08 17:45:47.585213 windmill_api-1.96.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-08 17:45:47.581213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-08 17:45:47.641213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-08 17:45:47.629213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-08 17:45:47.677214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-08 17:45:47.681213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-08 17:45:20.993151 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-08 17:45:47.717213 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-08 17:45:21.917153 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-08 17:45:47.725214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-08 17:45:47.757214 windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-08 17:45:47.841214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-08 17:45:47.813214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-08 17:45:47.917214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-08 17:45:47.893214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-08 17:45:47.933214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 17:45:21.625152 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-08 17:45:47.957214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 17:45:20.753150 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-08 17:45:47.981214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-08 17:45:47.997214 windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-08 17:45:48.041214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-08 17:45:48.025214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-08 17:45:48.085214 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-08 17:45:48.257215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-08 17:45:48.145215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-08 17:45:48.185215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-08 17:45:48.233215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-08 17:45:48.277215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-08 17:45:20.877150 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-08 17:45:48.313215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 17:45:20.825150 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-08 17:45:48.321215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-08 17:45:48.365215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-08 17:45:48.513215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-08 17:45:48.429215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-08 17:45:48.473215 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-08 17:45:48.521216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-08 17:45:48.557216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-08 17:45:48.573216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:22.069154 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-08 17:45:48.601216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-08 17:45:48.621216 windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-08 17:45:48.645216 windmill_api-1.96.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-08 17:45:48.673216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-08 17:45:48.689216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 17:45:20.929150 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-08 17:45:48.717216 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 17:45:20.721150 windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-08 17:45:21.009151 windmill_api-1.96.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-08 17:45:48.749216 windmill_api-1.96.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-08 17:45:48.861216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-08 17:45:48.793216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 17:45:21.953153 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 17:45:48.833216 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 17:45:21.389151 windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-08 17:45:21.429152 windmill_api-1.96.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-08 17:45:48.905216 windmill_api-1.96.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-08 17:45:22.089154 windmill_api-1.96.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-08 17:45:48.897216 windmill_api-1.96.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-08 17:45:48.929216 windmill_api-1.96.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-08 17:45:48.961217 windmill_api-1.96.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-08 17:45:48.961217 windmill_api-1.96.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-08 17:45:21.857153 windmill_api-1.96.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-08 17:45:49.005217 windmill_api-1.96.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-08 17:45:49.021217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-08 17:45:49.093217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-08 17:45:20.733150 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-08 17:45:49.065217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-08 17:45:49.101217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-08 17:45:49.133217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-08 17:45:49.157217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-08 17:45:21.741152 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-08 17:45:49.169217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-08 17:45:49.209217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-08 17:45:20.561150 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-08 17:45:49.205217 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-08 17:45:21.981153 windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-08 17:45:49.485218 windmill_api-1.96.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-08 17:45:49.237217 windmill_api-1.96.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-08 17:45:49.301217 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-08 17:45:49.429218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-08 17:45:49.557218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 17:45:49.529218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-08 17:45:21.429152 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-08 17:45:49.565218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-08 17:45:49.613218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-08 17:45:21.457152 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-08 17:45:49.685218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-08 17:45:49.657218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 17:45:49.701218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-08 17:45:20.845150 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-08 17:45:49.725218 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-08 17:45:49.765219 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-08 17:45:20.549150 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-08 17:45:49.869219 windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-08 17:45:21.829153 windmill_api-1.96.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.049151 windmill_api-1.96.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-08 17:45:49.829219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-08 17:45:49.945219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-08 17:45:49.925219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-08 17:45:49.969219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-08 17:45:49.989219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-08 17:45:50.009219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:21.605152 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 17:45:50.037219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:45:21.517152 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 17:45:50.053219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-08 17:45:50.085219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-08 17:45:50.165219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-08 17:45:50.141219 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-08 17:45:50.285220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-08 17:45:50.213220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-08 17:45:50.269220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 17:45:21.817153 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-08 17:45:50.317220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 17:45:21.353151 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-08 17:45:50.329220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-08 17:45:50.357220 windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-08 17:45:50.397220 windmill_api-1.96.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-08 17:45:50.409220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-08 17:45:50.437220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-08 17:45:21.381152 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-08 17:45:50.537220 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-08 17:45:21.297151 windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:45:21.973153 windmill_api-1.96.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-08 17:45:20.585150 windmill_api-1.96.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-08 17:45:50.477220 windmill_api-1.96.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-08 17:45:50.517220 windmill_api-1.96.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      328 2023-05-08 17:45:21.113151 windmill_api-1.96.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-08 17:45:50.561221 windmill_api-1.96.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-08 17:45:50.577221 windmill_api-1.96.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-08 17:45:50.633221 windmill_api-1.96.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-08 17:45:50.605221 windmill_api-1.96.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-08 17:45:50.653221 windmill_api-1.96.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-08 17:45:50.661221 windmill_api-1.96.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 17:45:50.681221 windmill_api-1.96.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-08 17:45:50.725221 windmill_api-1.96.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-08 17:45:50.729221 windmill_api-1.96.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-08 17:45:50.773221 windmill_api-1.96.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-08 17:45:50.757221 windmill_api-1.96.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-08 17:45:50.801221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-08 17:45:50.797221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 17:45:50.857221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-08 17:45:50.913221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-08 17:45:50.913221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-08 17:45:50.957221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-08 17:45:50.965222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-08 17:45:51.001222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 17:45:20.789150 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 17:45:51.005221 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 17:45:20.713150 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-08 17:45:51.061222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-08 17:45:51.049222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-08 17:45:51.241222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-08 17:45:51.125222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-08 17:45:51.169222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-08 17:45:51.321222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-08 17:45:51.285222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 17:45:21.901153 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-08 17:45:51.333222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 17:45:21.657152 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-08 17:45:51.361222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-08 17:45:51.377222 windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-08 17:45:51.389222 windmill_api-1.96.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-08 17:45:51.405223 windmill_api-1.96.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-08 17:45:51.445223 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-08 17:45:51.433223 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-08 17:45:21.785153 windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-08 17:45:51.465223 windmill_api-1.96.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-08 17:45:51.473223 windmill_api-1.96.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-08 17:45:21.721152 windmill_api-1.96.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-08 17:45:51.553223 windmill_api-1.96.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-08 17:45:51.505223 windmill_api-1.96.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-08 17:45:51.533223 windmill_api-1.96.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-08 17:45:51.669223 windmill_api-1.96.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-08 17:45:51.581223 windmill_api-1.96.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-08 17:45:51.609223 windmill_api-1.96.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-08 17:45:21.605152 windmill_api-1.96.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-08 17:45:21.909153 windmill_api-1.96.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-08 17:45:51.645223 windmill_api-1.96.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-08 17:45:51.677223 windmill_api-1.96.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-08 17:45:51.697223 windmill_api-1.96.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-08 17:45:51.721223 windmill_api-1.96.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-08 17:45:51.741223 windmill_api-1.96.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-08 17:45:51.769223 windmill_api-1.96.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      209 2023-05-08 17:45:21.805153 windmill_api-1.96.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-08 17:45:51.785223 windmill_api-1.96.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-08 17:45:21.481152 windmill_api-1.96.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-08 17:45:51.825224 windmill_api-1.96.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-08 17:45:51.849223 windmill_api-1.96.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-08 17:45:51.873224 windmill_api-1.96.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      211 2023-05-08 17:45:21.745153 windmill_api-1.96.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-08 17:45:51.909224 windmill_api-1.96.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 17:45:52.033224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 17:45:21.233151 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 17:45:51.945224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 17:45:51.977224 windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-08 17:45:52.153224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-08 17:45:52.069224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-08 17:45:52.129224 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-08 17:45:52.245225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-08 17:45:52.213225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-08 17:45:52.257225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-08 17:45:52.293225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-08 17:45:52.305225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 17:45:21.765153 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-08 17:45:52.333225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 17:45:21.961153 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-08 17:45:52.345225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-08 17:45:52.377225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-08 17:45:52.469225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-08 17:45:52.437225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-08 17:45:52.477225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-08 17:45:52.521225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-08 17:45:52.517225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-08 17:45:21.349151 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-08 17:45:52.557225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-08 17:45:21.613152 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-08 17:45:52.561225 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-08 17:45:52.597226 windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-08 17:45:52.605225 windmill_api-1.96.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-08 17:45:52.737226 windmill_api-1.96.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-08 17:45:52.649226 windmill_api-1.96.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-08 17:45:52.789226 windmill_api-1.96.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     1985 2023-05-08 17:45:52.785226 windmill_api-1.96.0/windmill_api/models/update_raw_app_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-08 17:45:52.837226 windmill_api-1.96.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-08 17:45:52.833226 windmill_api-1.96.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-08 17:45:52.869226 windmill_api-1.96.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-08 17:45:52.881226 windmill_api-1.96.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 17:45:52.905226 windmill_api-1.96.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-08 17:45:52.929226 windmill_api-1.96.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-08 17:45:52.957226 windmill_api-1.96.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-08 17:45:52.969226 windmill_api-1.96.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-08 17:45:53.045226 windmill_api-1.96.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-08 17:45:53.001226 windmill_api-1.96.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-08 17:45:53.045226 windmill_api-1.96.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-08 17:45:53.085227 windmill_api-1.96.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-08 17:45:53.137227 windmill_api-1.96.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-08 17:45:53.121227 windmill_api-1.96.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-08 17:45:53.209227 windmill_api-1.96.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-08 17:45:53.177227 windmill_api-1.96.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-08 17:45:53.233227 windmill_api-1.96.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-08 17:45:53.257227 windmill_api-1.96.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-08 17:45:53.277227 windmill_api-1.96.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-08 17:45:08.361165 windmill_api-1.96.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-08 17:45:53.281227 windmill_api-1.96.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.0/PKG-INFO
```

### Comparing `windmill_api-1.95.1/LICENSE` & `windmill_api-1.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/README.md` & `windmill_api-1.96.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/create_app.py` & `windmill_api-1.96.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/delete_app.py` & `windmill_api-1.96.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/execute_component.py` & `windmill_api-1.96.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/exists_app.py` & `windmill_api-1.96.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.96.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.96.0/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.96.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.96.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.96.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.96.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/list_apps.py` & `windmill_api-1.96.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.96.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/app/update_app.py` & `windmill_api-1.96.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.96.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.96.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/capture/create_capture.py` & `windmill_api-1.96.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/capture/get_capture.py` & `windmill_api-1.96.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/capture/update_capture.py` & `windmill_api-1.96.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/draft/create_draft.py` & `windmill_api-1.96.0/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/favorite/star.py` & `windmill_api-1.96.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/favorite/unstar.py` & `windmill_api-1.96.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/create_flow.py` & `windmill_api-1.96.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.96.0/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.96.0/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.96.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.96.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/list_flows.py` & `windmill_api-1.96.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.96.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/flow/update_flow.py` & `windmill_api-1.96.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/create_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/get_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.96.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.96.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/list_folders.py` & `windmill_api-1.96.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/folder/update_folder.py` & `windmill_api-1.96.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.96.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.96.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.96.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.96.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/create_group.py` & `windmill_api-1.96.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/delete_group.py` & `windmill_api-1.96.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/get_group.py` & `windmill_api-1.96.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/list_group_names.py` & `windmill_api-1.96.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/list_groups.py` & `windmill_api-1.96.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.96.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/group/update_group.py` & `windmill_api-1.96.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/input_/create_input.py` & `windmill_api-1.96.0/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/input_/delete_input.py` & `windmill_api-1.96.0/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.96.0/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.96.0/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/input_/update_input.py` & `windmill_api-1.96.0/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.96.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.96.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.96.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.96.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.96.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.96.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.96.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_job.py` & `windmill_api-1.96.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.96.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.96.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.96.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.96.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/list_jobs.py` & `windmill_api-1.96.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/list_queue.py` & `windmill_api-1.96.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/result_by_id.py` & `windmill_api-1.96.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.96.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.96.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.96.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.96.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.96.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.96.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.96.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/create_account.py` & `windmill_api-1.96.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.96.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.96.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.96.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.96.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/create_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/get_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.96.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/list_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.96.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/update_resource.py` & `windmill_api-1.96.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.96.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.96.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.96.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.96.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.96.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.96.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.96.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/create_script.py` & `windmill_api-1.96.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.96.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.96.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.96.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.96.0/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.96.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.96.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.96.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.96.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/list_scripts.py` & `windmill_api-1.96.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.96.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.96.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/settings/backend_version.py` & `windmill_api-1.96.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.96.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/accept_invite.py` & `windmill_api-1.96.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/create_token.py` & `windmill_api-1.96.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.96.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/create_user.py` & `windmill_api-1.96.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.96.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/decline_invite.py` & `windmill_api-1.96.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/delete_token.py` & `windmill_api-1.96.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/delete_user.py` & `windmill_api-1.96.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/get_current_email.py` & `windmill_api-1.96.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/get_usage.py` & `windmill_api-1.96.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.96.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/global_user_update.py` & `windmill_api-1.96.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/global_whoami.py` & `windmill_api-1.96.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.96.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.96.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/list_tokens.py` & `windmill_api-1.96.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/list_usernames.py` & `windmill_api-1.96.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/list_users.py` & `windmill_api-1.96.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.96.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.96.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/login.py` & `windmill_api-1.96.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.96.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/logout.py` & `windmill_api-1.96.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/set_password.py` & `windmill_api-1.96.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/update_user.py` & `windmill_api-1.96.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/whoami.py` & `windmill_api-1.96.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/user/whois.py` & `windmill_api-1.96.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/create_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/get_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.96.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/list_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/variable/update_variable.py` & `windmill_api-1.96.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.96.0/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/worker/list_workers.py` & `windmill_api-1.96.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/add_user.py` & `windmill_api-1.96.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.96.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.96.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.96.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.96.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.96.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.96.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.96.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.96.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.96.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.96.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.96.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.96.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.96.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.96.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.96.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.96.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.96.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/client.py` & `windmill_api-1.96.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.96.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.96.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.96.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/add_user_json_body.py` & `windmill_api-1.96.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.96.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.96.0/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/audit_log.py` & `windmill_api-1.96.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/audit_log_operation.py` & `windmill_api-1.96.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.96.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all.py` & `windmill_api-1.96.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one.py` & `windmill_api-1.96.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.96.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.96.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job.py` & `windmill_api-1.96.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_args.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.96.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.96.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.96.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/contextual_variable.py` & `windmill_api-1.96.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_account_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_app_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_group_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_input.py` & `windmill_api-1.96.0/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_input_args.py` & `windmill_api-1.96.0/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_input_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.96.0/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_resource.py` & `windmill_api-1.96.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.96.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_script_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.96.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_token_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_user_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_variable.py` & `windmill_api-1.96.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_workspace.py` & `windmill_api-1.96.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.96.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.96.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.96.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.96.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_resource.py` & `windmill_api-1.96.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_resource_type.py` & `windmill_api-1.96.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_schedule.py` & `windmill_api-1.96.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.96.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.96.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_variable.py` & `windmill_api-1.96.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.96.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.96.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.96.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.96.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.96.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.96.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.96.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow.py` & `windmill_api-1.96.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_metadata.py` & `windmill_api-1.96.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module.py` & `windmill_api-1.96.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.96.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_args.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_schema.py` & `windmill_api-1.96.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status.py` & `windmill_api-1.96.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_module.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value.py` & `windmill_api-1.96.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/folder.py` & `windmill_api-1.96.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.96.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.96.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_group_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_job_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.96.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.96.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.96.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/global_user_info.py` & `windmill_api-1.96.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.96.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.96.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/group.py` & `windmill_api-1.96.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/group_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/identity.py` & `windmill_api-1.96.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/input_.py` & `windmill_api-1.96.0/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/input_args.py` & `windmill_api-1.96.0/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.96.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.96.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.96.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/javascript_transform.py` & `windmill_api-1.96.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/job.py` & `windmill_api-1.96.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.96.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.96.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.96.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.96.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.96.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.96.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_app.py` & `windmill_api-1.96.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_resource.py` & `windmill_api-1.96.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_variable.py` & `windmill_api-1.96.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/login.py` & `windmill_api-1.96.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/login_json_body.py` & `windmill_api-1.96.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.96.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_schedule.py` & `windmill_api-1.96.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_schedule_args.py` & `windmill_api-1.96.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script.py` & `windmill_api-1.96.0/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script_schema.py` & `windmill_api-1.96.0/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.96.0/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.96.0/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_token.py` & `windmill_api-1.96.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.96.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/new_user.py` & `windmill_api-1.96.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow.py` & `windmill_api-1.96.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_schema.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_flow.py` & `windmill_api-1.96.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_script.py` & `windmill_api-1.96.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/policy.py` & `windmill_api-1.96.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/preview.py` & `windmill_api-1.96.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/preview_args.py` & `windmill_api-1.96.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.96.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job.py` & `windmill_api-1.96.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_args.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/raw_script.py` & `windmill_api-1.96.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.96.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.96.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.96.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.96.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/resource.py` & `windmill_api-1.96.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/resource_type.py` & `windmill_api-1.96.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.96.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.96.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/retry.py` & `windmill_api-1.96.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.96.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.96.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/schedule.py` & `windmill_api-1.96.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/schedule_args.py` & `windmill_api-1.96.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/script.py` & `windmill_api-1.96.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/script_args.py` & `windmill_api-1.96.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/script_extra_perms.py` & `windmill_api-1.96.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/script_schema.py` & `windmill_api-1.96.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/set_password_json_body.py` & `windmill_api-1.96.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.96.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/slack_token.py` & `windmill_api-1.96.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/slack_token_bot.py` & `windmill_api-1.96.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/star_json_body.py` & `windmill_api-1.96.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/static_transform.py` & `windmill_api-1.96.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/token_response.py` & `windmill_api-1.96.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/truncated_token.py` & `windmill_api-1.96.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/unstar_json_body.py` & `windmill_api-1.96.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_app_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_group_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_input.py` & `windmill_api-1.96.0/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_input_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.96.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_user_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.96.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/usage.py` & `windmill_api-1.96.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/user.py` & `windmill_api-1.96.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/user_usage.py` & `windmill_api-1.96.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/user_workspace_list.py` & `windmill_api-1.96.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.96.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/whoami_response_200.py` & `windmill_api-1.96.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.96.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/whois_response_200.py` & `windmill_api-1.96.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.96.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/worker_ping.py` & `windmill_api-1.96.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/workspace.py` & `windmill_api-1.96.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/models/workspace_invite.py` & `windmill_api-1.96.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/windmill_api/types.py` & `windmill_api-1.96.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.1/setup.py` & `windmill_api-1.96.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  'windmill_api.api.flow',
  'windmill_api.api.folder',
  'windmill_api.api.granular_acl',
  'windmill_api.api.group',
  'windmill_api.api.input_',
  'windmill_api.api.job',
  'windmill_api.api.oauth',
+ 'windmill_api.api.raw_app',
  'windmill_api.api.resource',
  'windmill_api.api.schedule',
  'windmill_api.api.script',
  'windmill_api.api.settings',
  'windmill_api.api.user',
  'windmill_api.api.variable',
  'windmill_api.api.worker',
@@ -30,15 +31,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.95.1',
+    'version': '1.96.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.95.1/PKG-INFO` & `windmill_api-1.96.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.95.1
+Version: 1.96.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


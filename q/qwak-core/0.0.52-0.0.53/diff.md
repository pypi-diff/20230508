# Comparing `tmp/qwak_core-0.0.52.tar.gz` & `tmp/qwak_core-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.52.tar", max compression
+gzip compressed data, was "qwak_core-0.0.53.tar", max compression
```

## Comparing `qwak_core-0.0.52.tar` & `qwak_core-0.0.53.tar`

### file list

```diff
@@ -1,570 +1,570 @@
--rw-r--r--   0        0        0      264 2023-05-04 13:12:04.738172 qwak_core-0.0.52/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:13:47.546764 qwak_core-0.0.52/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-04 13:13:47.574764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-04 13:13:26.286641 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.574764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-04 13:13:47.570764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-04 13:13:25.886638 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.570764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-04 13:13:47.570764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-04 13:13:26.074639 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.574764 qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-04 13:13:47.562764 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-04 13:13:25.330635 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-04 13:13:47.562764 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-04 13:13:47.566763 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-04 13:13:25.518636 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.566763 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-04 13:13:47.566763 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-04 13:13:25.702637 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.570764 qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-04 13:13:47.550763 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-04 13:13:25.134634 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-04 13:13:47.550763 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-04 13:13:47.550763 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-04 13:13:26.478642 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.554764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-04 13:13:47.554764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-04 13:13:26.854644 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.558764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-04 13:13:47.558764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-04 13:13:27.042645 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-04 13:13:47.558764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-04 13:13:47.554764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-04 13:13:26.666643 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.554764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-04 13:13:47.562764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-04 13:13:27.246646 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.562764 qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-04 13:13:47.606764 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-04 13:13:29.946662 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.606764 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-04 13:13:47.606764 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-04 13:13:30.138663 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-04 13:13:47.610764 qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-04 13:13:47.678764 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-04 13:13:35.794695 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.682764 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-04 13:13:47.682764 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-04 13:13:35.986697 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-04 13:13:47.682764 qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-04 13:13:47.686764 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-04 13:13:36.974702 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-04 13:13:47.686764 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-04 13:13:47.686764 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-04 13:13:36.786701 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.686764 qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-04 13:13:47.690764 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-04 13:13:37.170704 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.690764 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-04 13:13:47.690764 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-04 13:13:37.358704 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-04 13:13:47.690764 qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-04 13:13:47.754765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-04 13:13:42.890736 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.754765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-04 13:13:47.750765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-04 13:13:42.510734 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.750765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-04 13:13:47.750765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-04 13:13:42.698735 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.754765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-04 13:13:47.746765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-04 13:13:42.126732 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-04 13:13:47.746765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-04 13:13:47.746765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-04 13:13:42.322733 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.750765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-04 13:13:47.762765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-04 13:13:43.446740 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.762765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-04 13:13:47.758765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-04 13:13:43.262739 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.758765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-04 13:13:47.754765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-04 13:13:43.074738 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.758765 qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-04 13:13:47.802765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-04 13:13:46.890760 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.802765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-04 13:13:47.798765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-04 13:13:46.498757 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.798765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-04 13:13:47.798765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-04 13:13:46.698758 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-04 13:13:47.798765 qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-04 13:13:47.718764 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-04 13:13:39.390716 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-04 13:13:47.718764 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-04 13:13:47.714764 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-04 13:13:39.194715 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.718764 qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-04 13:13:47.706764 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-04 13:13:38.766713 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.706764 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-04 13:13:47.710765 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-04 13:13:38.994714 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.710765 qwak_core-0.0.52/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-04 13:13:47.710765 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-04 13:13:39.590717 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-04 13:13:47.714764 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-04 13:13:47.714764 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-04 13:13:40.010720 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-04 13:13:47.714764 qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-04 13:13:47.726765 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-04 13:13:40.410722 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.726765 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-04 13:13:47.726765 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-04 13:13:40.598723 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-04 13:13:47.726765 qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-04 13:13:47.698764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-04 13:13:38.166709 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.702764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-04 13:13:47.702764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-04 13:13:38.366710 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-04 13:13:47.702764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-04 13:13:47.694764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-04 13:13:37.758707 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.698764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-04 13:13:47.694764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-04 13:13:37.566706 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.694764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-04 13:13:47.698764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-04 13:13:37.962708 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-04 13:13:47.698764 qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-04 13:13:47.594764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-04 13:13:28.986656 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.594764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-04 13:13:47.598764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-04 13:13:29.174657 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.598764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-04 13:13:47.598764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-04 13:13:29.366658 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-04 13:13:47.602764 qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-04 13:13:47.658764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-04 13:13:34.614688 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.662764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-04 13:13:47.658764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-04 13:13:34.418687 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-04 13:13:47.658764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-04 13:13:47.638764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-04 13:13:32.674677 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.638764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-04 13:13:47.634764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-04 13:13:32.486676 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.634764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-04 13:13:47.626764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-04 13:13:31.898673 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.630764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-04 13:13:47.630764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-04 13:13:32.298675 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-04 13:13:47.634764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-04 13:13:47.638764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-04 13:13:32.862678 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.638764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-04 13:13:47.642764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-04 13:13:33.058680 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-04 13:13:47.642764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25213 2023-05-04 13:13:47.630764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37366 2023-05-04 13:13:32.098674 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.630764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-04 13:13:47.642764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-04 13:13:33.246681 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.646764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     5958 2023-05-04 13:13:47.646764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
--rw-r--r--   0        0        0     6232 2023-05-04 13:13:33.438682 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.646764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-04 13:13:47.662764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-04 13:13:47.082761 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.662764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-04 13:13:47.662764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-04 13:13:47.274762 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-04 13:13:47.666764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-04 13:13:47.666764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-04 13:13:35.206692 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.666764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-04 13:13:47.670764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-04 13:13:35.398693 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-04 13:13:47.670764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-04 13:13:47.670764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-04 13:13:35.602694 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.670764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-04 13:13:47.674764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-04 13:13:36.382699 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.678764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-04 13:13:47.674764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-04 13:13:36.178698 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-04 13:13:47.674764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-04 13:13:47.678764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-04 13:13:36.590700 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.678764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-04 13:13:47.646764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-04 13:13:33.634683 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.650764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-04 13:13:47.650764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-04 13:13:33.834684 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.650764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-04 13:13:47.654764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-04 13:13:34.026685 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-04 13:13:47.654764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-04 13:13:47.654764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-04 13:13:34.222686 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.654764 qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-04 13:13:47.762765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-04 13:13:43.630741 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.762765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-04 13:13:47.766765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-04 13:13:43.814742 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-04 13:13:47.766765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-04 13:13:47.766765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-04 13:13:43.998743 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.770765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-04 13:13:47.770765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-04 13:13:44.194744 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-04 13:13:47.770765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-04 13:13:47.770765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-04 13:13:44.390745 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-04 13:13:47.774765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-04 13:13:47.774765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-04 13:13:44.578746 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.774765 qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-04 13:13:47.730764 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-04 13:13:40.786724 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.730764 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-04 13:13:47.730764 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-04 13:13:40.978726 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-04 13:13:47.734765 qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-04 13:13:47.610764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-04 13:13:31.066668 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.614764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-04 13:13:47.618764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-04 13:13:31.290669 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.618764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-04 13:13:47.622764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-04 13:13:31.482670 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-04 13:13:47.622764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-04 13:13:47.626764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-04 13:13:31.674672 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.626764 qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-04 13:13:47.706764 qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-04 13:13:38.566712 qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-04 13:13:47.706764 qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-04 13:13:47.774765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-04 13:13:44.766747 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.778765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-04 13:13:47.778765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-04 13:13:44.950749 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.778765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-04 13:13:47.782765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-04 13:13:45.138749 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.782765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-04 13:13:47.782765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-04 13:13:45.330751 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.782765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-04 13:13:47.786765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-04 13:13:45.526752 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.786765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-04 13:13:47.786765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-04 13:13:45.734753 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-04 13:13:47.790765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-04 13:13:47.790765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-04 13:13:45.926754 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.790765 qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-04 13:13:47.734765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-04 13:13:41.358728 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.738765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-04 13:13:47.742765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-04 13:13:41.934731 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.742765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-04 13:13:47.738765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-04 13:13:41.550729 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-04 13:13:47.738765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-04 13:13:47.738765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-04 13:13:41.738730 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.742765 qwak_core-0.0.52/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-04 13:13:47.722765 qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-04 13:13:40.214721 qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-04 13:13:47.722765 qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-04 13:13:47.590764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-04 13:13:30.602665 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-04 13:13:47.590764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-04 13:13:47.586764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-04 13:13:30.362664 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.590764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-04 13:13:47.594764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-04 13:13:30.842667 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-04 13:13:47.594764 qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-04 13:13:47.722765 qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-04 13:13:39.798719 qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-04 13:13:47.722765 qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-04 13:13:47.734765 qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-04 13:13:41.170727 qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-04 13:13:47.734765 qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-04 13:13:47.586764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-04 13:13:28.202652 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.586764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-04 13:13:47.582764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-04 13:13:28.014650 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-04 13:13:47.586764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-04 13:13:47.578764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-04 13:13:27.434647 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.578764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-04 13:13:47.578764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-04 13:13:27.626648 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.578764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-04 13:13:47.582764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-04 13:13:27.814649 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-04 13:13:47.582764 qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-04 13:13:47.794765 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-04 13:13:46.310756 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-04 13:13:47.794765 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-04 13:13:47.790765 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-04 13:13:46.118755 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.794765 qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-04 13:13:47.602764 qwak_core-0.0.52/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-04 13:13:29.562659 qwak_core-0.0.52/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.602764 qwak_core-0.0.52/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-04 13:13:47.602764 qwak_core-0.0.52/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-04 13:13:29.754660 qwak_core-0.0.52/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-04 13:13:47.606764 qwak_core-0.0.52/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-04 13:13:49.890777 qwak_core-0.0.52/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-04 13:13:49.890777 qwak_core-0.0.52/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-04 13:12:04.738172 qwak_core-0.0.52/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9275 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.742172 qwak_core-0.0.52/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-04 13:12:04.746172 qwak_core-0.0.52/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.52/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-08 09:17:44.147743 qwak_core-0.0.53/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 09:19:32.672442 qwak_core-0.0.53/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-08 09:19:10.208298 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-08 09:19:09.812295 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-08 09:19:10.008296 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-08 09:19:09.220291 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-08 09:19:09.416292 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-08 09:19:09.620294 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-08 09:19:09.020290 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-08 09:19:10.408299 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-08 09:19:10.792301 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-08 09:19:11.004303 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-08 09:19:10.600300 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-08 09:19:11.212304 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-08 09:19:14.240323 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-08 09:19:32.736442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-08 09:19:14.488325 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-08 09:19:32.736442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-08 09:19:20.324362 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-08 09:19:20.536364 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-08 09:19:21.560370 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-08 09:19:21.364369 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-08 09:19:21.752372 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-08 09:19:21.948373 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-08 09:19:27.712410 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-08 09:19:27.296407 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-08 09:19:27.512408 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-08 09:19:26.884405 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-08 09:19:27.092406 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-08 09:19:28.316413 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-08 09:19:28.120412 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-08 09:19:27.916411 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-08 09:19:31.920437 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.944443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-08 09:19:31.528434 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-05-08 09:19:31.728435 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-08 09:19:24.000386 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-08 09:19:23.800385 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-08 09:19:23.412382 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-08 09:19:23.604383 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-08 09:19:24.208387 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-08 09:19:32.848443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-08 09:19:24.640390 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-08 09:19:25.068393 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-08 09:19:25.272394 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-08 09:19:22.776378 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-08 09:19:22.980379 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-08 09:19:22.352375 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-08 09:19:22.156374 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-08 09:19:22.572377 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-08 09:19:13.100316 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-08 09:19:13.328317 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-08 09:19:13.580319 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-08 09:19:19.120355 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-08 09:19:18.920354 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-08 09:19:17.140342 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-08 09:19:16.940341 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-08 09:19:16.308337 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-08 09:19:16.744340 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-08 09:19:17.336343 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-08 09:19:17.528344 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-08 09:19:16.528338 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-08 09:19:17.724346 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-08 09:19:17.932347 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-08 09:19:32.120438 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-08 09:19:32.316439 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-08 09:19:19.732359 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-08 09:19:19.932360 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-08 09:19:20.132361 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-08 09:19:20.960367 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-08 09:19:20.748365 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-08 09:19:21.160368 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-08 09:19:18.144348 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-08 09:19:18.336350 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-08 09:19:18.528351 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-08 09:19:18.720352 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-08 09:19:28.524415 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-08 09:19:28.720416 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-08 09:19:28.932417 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-08 09:19:29.140419 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-08 09:19:29.356420 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-08 09:19:29.552421 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-08 09:19:25.472396 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-08 09:19:25.668397 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-08 09:19:15.432331 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-08 09:19:15.660333 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.744442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-08 09:19:32.744442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-08 09:19:15.872334 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-08 09:19:32.752442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-08 09:19:16.084335 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-08 09:19:23.188381 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-08 09:19:29.752423 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-08 09:19:29.948424 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-08 09:19:30.152425 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-08 09:19:30.348427 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-08 09:19:30.548428 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-08 09:19:30.756429 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-08 09:19:30.944430 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-08 09:19:26.092399 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-08 09:19:26.688403 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-08 09:19:26.292401 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-08 09:19:26.488402 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-08 09:19:24.864391 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-08 09:19:14.932328 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-08 09:19:14.708326 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-08 09:19:15.156329 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-08 09:19:24.424389 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-08 09:19:25.872398 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-08 09:19:12.220310 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-08 09:19:12.024309 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-08 09:19:11.416305 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-08 09:19:11.616307 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-08 09:19:11.816308 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-08 09:19:31.336433 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-08 09:19:31.144432 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-08 09:19:13.796321 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-08 09:19:14.020322 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-08 09:19:34.404453 qwak_core-0.0.53/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 09:19:34.404453 qwak_core-0.0.53/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.53/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.53/PKG-INFO
```

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/pyproject.toml` & `qwak_core-0.0.53/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.52"
+version = "0.0.53"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.52/qwak/automations/__init__.py` & `qwak_core-0.0.53/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/automations/automation_executions.py` & `qwak_core-0.0.53/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/automations/automations.py` & `qwak_core-0.0.53/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.53/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.53/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.53/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.53/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.53/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/alert_management/client.py` & `qwak_core-0.0.53/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/analytics/client.py` & `qwak_core-0.0.53/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/audience/client.py` & `qwak_core-0.0.53/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/automation_management/client.py` & `qwak_core-0.0.53/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.53/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.53/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.53/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.53/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/build_management/client.py` & `qwak_core-0.0.53/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.53/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.53/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/deployment/client.py` & `qwak_core-0.0.53/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.53/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.53/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.53/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.53/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.53/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/logging_client/client.py` & `qwak_core-0.0.53/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/model_management/client.py` & `qwak_core-0.0.53/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/project/client.py` & `qwak_core-0.0.53/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/secret_service/client.py` & `qwak_core-0.0.53/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.53/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.53/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.53/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.53/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.53/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.53/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.53/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.53/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.53/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/offline/client.py` & `qwak_core-0.0.53/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/feature_store/online/client.py` & `qwak_core-0.0.53/qwak/feature_store/online/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 from typing import TYPE_CHECKING, List, Optional
 
 from _qwak_proto.qwak.feature_store.serving.serving_pb2 import (
     BatchV1Feature as ServingProtoBatchV1Feature,
 )
 from _qwak_proto.qwak.feature_store.serving.serving_pb2 import (
     EntitiesHeader,
@@ -66,15 +65,15 @@
         self._serving_client = ServingServiceStub(channel)
 
     @staticmethod
     def to_string_entities_values(values) -> List[str]:
         return [str(value) for value in values]
 
     def get_feature_values(
-            self, schema: ModelSchema, df: "pd.DataFrame", model_name: str = "no-model"
+        self, schema: ModelSchema, df: "pd.DataFrame", model_name: str = "no-model"
     ) -> "pd.DataFrame":
         """
         :param schema: a ModelSchema object - defines the entities, features and prediction (irelevant in this case).
         :param df: a pandas data-frame with a column for each explicit feature needed
                          and a column for each entity key defined in the schema.
         :return: a pandas data-frame - the feature values defined in the schema
                                        of the requested entities in the df.
```

### Comparing `qwak_core-0.0.52/qwak/inner/const.py` & `qwak_core-0.0.53/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.53/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.53/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.53/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.53/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/singleton_meta.py` & `qwak_core-0.0.53/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/tool/auth.py` & `qwak_core-0.0.53/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.53/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.53/qwak/inner/tool/run_config/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         >>> validate_bool(True, False)
         True
         >>> validate_bool("true", False)
         False
         >>> validate_bool(None, True)
         False
     """
-    if value:
+    if value is not None:
         return isinstance(value, bool)
     elif is_required:
         return False
 
     return True
```

### Comparing `qwak_core-0.0.52/qwak/model/adapters/__init__.py` & `qwak_core-0.0.53/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.53/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.53/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.53/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.53/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.53/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/base.py` & `qwak_core-0.0.53/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/decorators/api.py` & `qwak_core-0.0.53/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.53/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/experiment_tracking.py` & `qwak_core-0.0.53/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/schema.py` & `qwak_core-0.0.53/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/schema_entities.py` & `qwak_core-0.0.53/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.53/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.53/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.53/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.53/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.53/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.53/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.53/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/client.py` & `qwak_core-0.0.53/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.53/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/models/model.py` & `qwak_core-0.0.53/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.53/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.53/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/tools/logger/logger.py` & `qwak_core-0.0.53/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak/tools/logger/logging.yml` & `qwak_core-0.0.53/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.53/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/qwak_services_mock/services_mock.py` & `qwak_core-0.0.53/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.52/setup.py` & `qwak_core-0.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.52',
+    'version': '0.0.53',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.52/PKG-INFO` & `qwak_core-0.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.52
+Version: 0.0.53
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```


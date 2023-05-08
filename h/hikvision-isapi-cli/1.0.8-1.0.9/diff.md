# Comparing `tmp/hikvision_isapi_cli-1.0.8.tar.gz` & `tmp/hikvision_isapi_cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikvision_isapi_cli-1.0.8.tar", max compression
+gzip compressed data, was "hikvision_isapi_cli-1.0.9.tar", max compression
```

## Comparing `hikvision_isapi_cli-1.0.8.tar` & `hikvision_isapi_cli-1.0.9.tar`

### file list

```diff
@@ -1,304 +1,304 @@
--rw-r--r--   0        0        0        0 2023-01-17 09:28:38.348946 hikvision_isapi_cli-1.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     3768 2023-01-17 09:21:44.810775 hikvision_isapi_cli-1.0.8/README.md
--rw-r--r--   0        0        0       24 2023-01-17 09:37:47.368937 hikvision_isapi_cli-1.0.8/docs/API.md
--rw-r--r--   0        0        0      105 2023-01-17 09:28:44.011639 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/__init__.py
--rw-r--r--   0        0        0       47 2023-01-17 09:28:41.487139 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 09:28:41.561189 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/__init__.py
--rw-r--r--   0        0        0     3809 2023-01-17 09:28:44.165751 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py
--rw-r--r--   0        0        0    13745 2023-01-17 09:28:44.205063 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py
--rw-r--r--   0        0        0     4919 2023-01-17 09:28:44.246344 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py
--rw-r--r--   0        0        0     3682 2023-01-17 09:28:44.223723 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_heartbeat.py
--rw-r--r--   0        0        0     7421 2023-01-17 09:28:44.296708 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_login.py
--rw-r--r--   0        0        0     4609 2023-01-17 10:22:12.718839 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_login_capabilities.py
--rw-r--r--   0        0        0        0 2023-01-17 09:28:41.505499 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/__init__.py
--rw-r--r--   0        0        0     4318 2023-01-17 09:28:44.295091 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/callstatus.py
--rw-r--r--   0        0        0     4624 2023-01-17 09:28:44.310084 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py
--rw-r--r--   0        0        0     4330 2023-01-17 09:28:44.326899 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilities.py
--rw-r--r--   0        0        0     2296 2023-01-17 09:28:44.310713 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilities1.py
--rw-r--r--   0        0        0     2285 2023-01-17 09:28:44.304335 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilties.py
--rw-r--r--   0        0        0     4379 2023-01-17 09:28:44.386660 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels.py
--rw-r--r--   0        0        0     2271 2023-01-17 09:28:44.322586 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels2.py
--rw-r--r--   0        0        0     5421 2023-01-17 09:28:44.464774 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py
--rw-r--r--   0        0        0     2578 2023-01-17 09:28:44.374131 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py
--rw-r--r--   0        0        0     4105 2023-01-17 09:28:44.429018 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_close.py
--rw-r--r--   0        0        0     4150 2023-01-17 09:28:44.420673 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_open.py
--rw-r--r--   0        0        0     2553 2023-01-17 09:28:44.362666 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_picture.py
--rw-r--r--   0        0        0     2902 2023-01-17 09:28:44.393953 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py
--rw-r--r--   0        0        0     2276 2023-01-17 09:28:44.362814 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceid.py
--rw-r--r--   0        0        0     2341 2023-01-17 09:28:44.369285 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py
--rw-r--r--   0        0        0     4226 2023-01-17 09:28:44.473777 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceinfo.py
--rw-r--r--   0        0        0     5497 2023-01-17 09:28:44.507906 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/door.py
--rw-r--r--   0        0        0     4442 2023-01-17 09:28:44.498441 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/door_capabilities.py
--rw-r--r--   0        0        0     2853 2023-01-17 09:28:44.466706 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/encryption_format_json.py
--rw-r--r--   0        0        0     4018 2023-01-17 09:28:44.464150 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py
--rw-r--r--   0        0        0     2257 2023-01-17 09:28:44.438111 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/index1.py
--rw-r--r--   0        0        0     4422 2023-01-17 09:28:44.508771 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/inputs_channels.py
--rw-r--r--   0        0        0     2262 2023-01-17 09:28:44.519160 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/status.py
--rw-r--r--   0        0        0     3554 2023-01-17 09:28:44.554694 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/usercheck.py
--rw-r--r--   0        0        0     2506 2023-01-17 09:28:44.513242 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/userpermission1.py
--rw-r--r--   0        0        0     2256 2023-01-17 09:28:44.506578 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/users.py
--rw-r--r--   0        0        0     2234 2023-01-17 10:17:26.800994 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/client.py
--rw-r--r--   0        0        0      282 2023-01-17 09:28:44.413275 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/errors.py
--rw-r--r--   0        0        0    62059 2023-01-17 09:28:43.126388 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/__init__.py
--rw-r--r--   0        0        0     2319 2023-01-17 09:28:44.557911 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_call_status.py
--rw-r--r--   0        0        0     1578 2023-01-17 09:28:44.517380 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py
--rw-r--r--   0        0        0     2477 2023-01-17 09:28:44.596931 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py
--rw-r--r--   0        0        0     2388 2023-01-17 09:28:44.620077 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py
--rw-r--r--   0        0        0     1749 2023-01-17 09:28:44.585989 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py
--rw-r--r--   0        0        0     4019 2023-01-17 09:28:44.697631 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_response_status.py
--rw-r--r--   0        0        0     6780 2023-01-17 09:28:44.632655 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py
--rw-r--r--   0        0        0   165585 2023-01-17 09:28:47.928951 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py
--rw-r--r--   0        0        0     5642 2023-01-17 09:28:44.719289 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py
--rw-r--r--   0        0        0     1763 2023-01-17 09:28:44.608416 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py
--rw-r--r--   0        0        0     1980 2023-01-17 09:28:44.620086 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py
--rw-r--r--   0        0        0     1526 2023-01-17 09:28:44.585205 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py
--rw-r--r--   0        0        0     3004 2023-01-17 09:28:44.658442 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py
--rw-r--r--   0        0        0     1702 2023-01-17 09:28:44.632498 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py
--rw-r--r--   0        0        0     1416 2023-01-17 09:28:44.603468 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py
--rw-r--r--   0        0        0     1426 2023-01-17 09:28:44.635169 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py
--rw-r--r--   0        0        0     1472 2023-01-17 09:28:44.631448 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py
--rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.661025 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py
--rw-r--r--   0        0        0     1449 2023-01-17 09:28:44.664678 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1523 2023-01-17 09:28:44.671433 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py
--rw-r--r--   0        0        0     1494 2023-01-17 09:28:44.672263 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py
--rw-r--r--   0        0        0     1456 2023-01-17 09:28:44.684836 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py
--rw-r--r--   0        0        0     1531 2023-01-17 09:28:44.700495 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py
--rw-r--r--   0        0        0     1531 2023-01-17 09:28:44.704043 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py
--rw-r--r--   0        0        0     1449 2023-01-17 09:28:44.714058 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py
--rw-r--r--   0        0        0     1464 2023-01-17 09:28:44.725640 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py
--rw-r--r--   0        0        0     1441 2023-01-17 09:28:44.726762 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py
--rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.736164 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py
--rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.759420 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py
--rw-r--r--   0        0        0     1484 2023-01-17 09:28:44.768894 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py
--rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.752142 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py
--rw-r--r--   0        0        0     1441 2023-01-17 09:28:44.771591 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py
--rw-r--r--   0        0        0     1456 2023-01-17 09:28:44.755495 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py
--rw-r--r--   0        0        0     1529 2023-01-17 09:28:44.778762 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.793587 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.794148 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py
--rw-r--r--   0        0        0     1534 2023-01-17 09:28:44.801996 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1519 2023-01-17 09:28:44.789440 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py
--rw-r--r--   0        0        0     1561 2023-01-17 09:28:44.790227 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py
--rw-r--r--   0        0        0     1541 2023-01-17 09:28:44.849609 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py
--rw-r--r--   0        0        0     1579 2023-01-17 09:28:44.789177 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py
--rw-r--r--   0        0        0     1489 2023-01-17 09:28:44.816126 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py
--rw-r--r--   0        0        0     1536 2023-01-17 09:28:44.807582 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.881162 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py
--rw-r--r--   0        0        0     1477 2023-01-17 09:28:44.843116 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1464 2023-01-17 09:28:44.844215 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py
--rw-r--r--   0        0        0     1539 2023-01-17 09:28:44.853548 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py
--rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.892166 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py
--rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.870941 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py
--rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.884542 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py
--rw-r--r--   0        0        0     1461 2023-01-17 09:28:44.919210 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.875298 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py
--rw-r--r--   0        0        0     1421 2023-01-17 09:28:44.871197 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py
--rw-r--r--   0        0        0     1544 2023-01-17 09:28:44.896393 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py
--rw-r--r--   0        0        0     1539 2023-01-17 09:28:44.891937 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.907613 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py
--rw-r--r--   0        0        0     1526 2023-01-17 09:28:44.945100 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py
--rw-r--r--   0        0        0     1524 2023-01-17 09:28:44.952479 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py
--rw-r--r--   0        0        0     1487 2023-01-17 09:28:44.953669 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py
--rw-r--r--   0        0        0     1467 2023-01-17 09:28:44.927748 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py
--rw-r--r--   0        0        0     1489 2023-01-17 09:28:44.968629 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py
--rw-r--r--   0        0        0     1474 2023-01-17 09:28:44.976680 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.013844 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py
--rw-r--r--   0        0        0     1474 2023-01-17 09:28:44.997502 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py
--rw-r--r--   0        0        0     1467 2023-01-17 09:28:45.001387 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py
--rw-r--r--   0        0        0     1449 2023-01-17 09:28:45.000540 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py
--rw-r--r--   0        0        0     1526 2023-01-17 09:28:45.008879 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py
--rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.003127 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py
--rw-r--r--   0        0        0     1426 2023-01-17 09:28:44.985372 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py
--rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.015304 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py
--rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.992737 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py
--rw-r--r--   0        0        0     1439 2023-01-17 09:28:45.021871 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py
--rw-r--r--   0        0        0     1472 2023-01-17 09:28:45.035228 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py
--rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.065123 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py
--rw-r--r--   0        0        0     1449 2023-01-17 09:28:45.058724 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py
--rw-r--r--   0        0        0     1524 2023-01-17 09:28:45.062420 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py
--rw-r--r--   0        0        0     1456 2023-01-17 09:28:45.084556 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py
--rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.113704 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py
--rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.091358 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py
--rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.108179 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py
--rw-r--r--   0        0        0     1477 2023-01-17 09:28:45.104285 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py
--rw-r--r--   0        0        0     1469 2023-01-17 09:28:45.069155 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py
--rw-r--r--   0        0        0     1484 2023-01-17 09:28:45.079718 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py
--rw-r--r--   0        0        0     1474 2023-01-17 09:28:45.133736 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py
--rw-r--r--   0        0        0     1482 2023-01-17 09:28:45.096529 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py
--rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.131052 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py
--rw-r--r--   0        0        0     1489 2023-01-17 09:28:45.126681 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py
--rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.155690 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py
--rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.136752 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py
--rw-r--r--   0        0        0     1469 2023-01-17 09:28:45.162768 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py
--rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.159455 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py
--rw-r--r--   0        0        0     1464 2023-01-17 09:28:45.179237 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py
--rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.182935 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py
--rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.178892 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py
--rw-r--r--   0        0        0     1474 2023-01-17 09:28:45.185641 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py
--rw-r--r--   0        0        0     1484 2023-01-17 09:28:45.195403 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py
--rw-r--r--   0        0        0     1431 2023-01-17 09:28:45.198666 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py
--rw-r--r--   0        0        0     1539 2023-01-17 09:28:45.217864 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py
--rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.222882 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py
--rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.222515 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py
--rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.224729 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1479 2023-01-17 09:28:45.229810 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py
--rw-r--r--   0        0        0     1477 2023-01-17 09:28:45.215842 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py
--rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.230514 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.236376 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py
--rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.250607 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py
--rw-r--r--   0        0        0     5455 2023-01-17 09:28:45.366437 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py
--rw-r--r--   0        0        0     1604 2023-01-17 09:28:45.255042 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py
--rw-r--r--   0        0        0     1599 2023-01-17 09:28:45.266895 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py
--rw-r--r--   0        0        0     3009 2023-01-17 09:28:45.312915 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py
--rw-r--r--   0        0        0     5227 2023-01-17 09:28:45.437027 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py
--rw-r--r--   0        0        0     1677 2023-01-17 09:28:45.293200 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py
--rw-r--r--   0        0        0     1927 2023-01-17 09:28:45.332567 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py
--rw-r--r--   0        0        0     1934 2023-01-17 09:28:45.323033 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py
--rw-r--r--   0        0        0     4548 2023-01-17 09:28:45.344849 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info.py
--rw-r--r--   0        0        0    31772 2023-01-17 09:28:46.707479 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py
--rw-r--r--   0        0        0    12689 2023-01-17 09:28:45.680285 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py
--rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.309553 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py
--rw-r--r--   0        0        0     1464 2023-01-17 09:28:45.308839 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.325592 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py
--rw-r--r--   0        0        0     1461 2023-01-17 09:28:45.325605 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py
--rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.338781 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py
--rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.352163 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py
--rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.366644 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py
--rw-r--r--   0        0        0     1526 2023-01-17 09:28:45.380821 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py
--rw-r--r--   0        0        0     3040 2023-01-17 09:28:45.457977 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py
--rw-r--r--   0        0        0     2645 2023-01-17 09:28:45.479705 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py
--rw-r--r--   0        0        0     1695 2023-01-17 09:28:45.397415 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py
--rw-r--r--   0        0        0     1848 2023-01-17 09:28:45.440252 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py
--rw-r--r--   0        0        0     1848 2023-01-17 09:28:45.434439 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py
--rw-r--r--   0        0        0     1706 2023-01-17 09:28:45.431562 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py
--rw-r--r--   0        0        0     1871 2023-01-17 09:28:45.456354 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py
--rw-r--r--   0        0        0     3132 2023-01-17 09:28:45.492249 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py
--rw-r--r--   0        0        0     2953 2023-01-17 09:28:45.478352 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py
--rw-r--r--   0        0        0     3208 2023-01-17 09:28:45.544013 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py
--rw-r--r--   0        0        0     7425 2023-01-17 09:28:45.735354 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py
--rw-r--r--   0        0        0     4767 2023-01-17 09:28:45.609815 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py
--rw-r--r--   0        0        0     1961 2023-01-17 09:28:45.544461 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py
--rw-r--r--   0        0        0     1752 2023-01-17 09:28:45.529158 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py
--rw-r--r--   0        0        0     3140 2023-01-17 09:28:45.603716 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py
--rw-r--r--   0        0        0     2544 2023-01-17 09:28:45.578190 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py
--rw-r--r--   0        0        0     1913 2023-01-17 09:28:45.564143 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py
--rw-r--r--   0        0        0     2803 2023-01-17 09:28:45.606574 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py
--rw-r--r--   0        0        0     2400 2023-01-17 09:28:45.609354 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py
--rw-r--r--   0        0        0     2690 2023-01-17 09:28:45.613220 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status.py
--rw-r--r--   0        0        0     2997 2023-01-17 09:28:45.624642 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py
--rw-r--r--   0        0        0     4161 2023-01-17 09:28:45.729227 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py
--rw-r--r--   0        0        0     3141 2023-01-17 09:28:45.708994 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py
--rw-r--r--   0        0        0     2719 2023-01-17 09:28:45.677094 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login.py
--rw-r--r--   0        0        0     2958 2023-01-17 09:28:45.685381 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py
--rw-r--r--   0        0        0     3693 2023-01-17 09:28:45.767088 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py
--rw-r--r--   0        0        0     2746 2023-01-17 09:28:45.714580 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py
--rw-r--r--   0        0        0     3581 2023-01-17 09:28:45.772521 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py
--rw-r--r--   0        0        0     3971 2023-01-17 09:28:45.798419 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py
--rw-r--r--   0        0        0     6459 2023-01-17 09:28:45.735364 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py
--rw-r--r--   0        0        0     2966 2023-01-17 09:28:45.745494 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py
--rw-r--r--   0        0        0     7988 2023-01-17 09:28:45.990228 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel.py
--rw-r--r--   0        0        0     7796 2023-01-17 09:28:45.912701 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio.py
--rw-r--r--   0        0        0     1478 2023-01-17 09:28:45.730947 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_compression_type.py
--rw-r--r--   0        0        0     1540 2023-01-17 09:28:45.750745 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_inbound_compression_type.py
--rw-r--r--   0        0        0     1995 2023-01-17 09:28:45.786244 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_voice_changer.py
--rw-r--r--   0        0        0     3132 2023-01-17 09:28:45.820585 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable.py
--rw-r--r--   0        0        0     8197 2023-01-17 09:28:46.107125 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel.py
--rw-r--r--   0        0        0     8968 2023-01-17 09:28:46.125763 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio.py
--rw-r--r--   0        0        0     1722 2023-01-17 09:28:45.810634 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_compression_type.py
--rw-r--r--   0        0        0     1760 2023-01-17 09:28:45.813507 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_inbound_compression_type.py
--rw-r--r--   0        0        0     2210 2023-01-17 09:28:45.847710 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_voice_changer.py
--rw-r--r--   0        0        0    12227 2023-01-17 09:28:46.276001 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport.py
--rw-r--r--   0        0        0     3726 2023-01-17 09:28:45.905456 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list.py
--rw-r--r--   0        0        0     4009 2023-01-17 09:28:45.886817 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol.py
--rw-r--r--   0        0        0     1914 2023-01-17 09:28:45.858021 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py
--rw-r--r--   0        0        0     8096 2023-01-17 09:28:46.159775 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast.py
--rw-r--r--   0        0        0     1800 2023-01-17 09:28:45.878574 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_active_multicast_enabled.py
--rw-r--r--   0        0        0     5373 2023-01-17 09:28:46.084313 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info.py
--rw-r--r--   0        0        0     1799 2023-01-17 09:28:45.910566 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py
--rw-r--r--   0        0        0     1768 2023-01-17 09:28:45.913968 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_ratio.py
--rw-r--r--   0        0        0     4229 2023-01-17 09:28:46.096223 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security.py
--rw-r--r--   0        0        0     2144 2023-01-17 09:28:45.979100 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security_security_algorithm.py
--rw-r--r--   0        0        0     2593 2023-01-17 09:28:46.060572 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_srtp_multicast.py
--rw-r--r--   0        0        0     4164 2023-01-17 09:28:46.137367 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast.py
--rw-r--r--   0        0        0     1760 2023-01-17 09:28:46.026195 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast_rtp_transport_type.py
--rw-r--r--   0        0        0    26045 2023-01-17 09:28:46.811142 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video.py
--rw-r--r--   0        0        0     1692 2023-01-17 09:28:45.994255 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_constant_bit_rate.py
--rw-r--r--   0        0        0     1765 2023-01-17 09:28:45.999781 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_intelligent_info_display_method.py
--rw-r--r--   0        0        0     1677 2023-01-17 09:28:46.114782 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_max_frame_rate.py
--rw-r--r--   0        0        0     1966 2023-01-17 09:28:46.165568 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_smart_codec.py
--rw-r--r--   0        0        0     2187 2023-01-17 09:28:46.184574 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_svc.py
--rw-r--r--   0        0        0     1672 2023-01-17 09:28:46.126741 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_lower_cap.py
--rw-r--r--   0        0        0     1672 2023-01-17 09:28:46.142200 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_upper_cap.py
--rw-r--r--   0        0        0     1687 2023-01-17 09:28:46.170829 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_codec_type.py
--rw-r--r--   0        0        0     1720 2023-01-17 09:28:46.171237 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_input_channel_id.py
--rw-r--r--   0        0        0     1740 2023-01-17 09:28:46.179507 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_quality_control_type.py
--rw-r--r--   0        0        0     1727 2023-01-17 09:28:46.194620 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_height.py
--rw-r--r--   0        0        0     1722 2023-01-17 09:28:46.237142 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_width.py
--rw-r--r--   0        0        0    10309 2023-01-17 09:28:46.511602 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport.py
--rw-r--r--   0        0        0     3241 2023-01-17 09:28:46.259865 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list.py
--rw-r--r--   0        0        0     3530 2023-01-17 09:28:46.328623 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol.py
--rw-r--r--   0        0        0     1729 2023-01-17 09:28:46.217905 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py
--rw-r--r--   0        0        0     7234 2023-01-17 09:28:46.516345 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast.py
--rw-r--r--   0        0        0     1580 2023-01-17 09:28:46.232355 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_active_multicast_enabled.py
--rw-r--r--   0        0        0     4535 2023-01-17 09:28:46.352913 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info.py
--rw-r--r--   0        0        0     1579 2023-01-17 09:28:46.258633 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py
--rw-r--r--   0        0        0     1548 2023-01-17 09:28:46.268360 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_ratio.py
--rw-r--r--   0        0        0     3749 2023-01-17 09:28:46.373824 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security.py
--rw-r--r--   0        0        0     1948 2023-01-17 09:28:46.371111 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security_security_algorithm.py
--rw-r--r--   0        0        0     2378 2023-01-17 09:28:46.335273 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_srtp_multicast.py
--rw-r--r--   0        0        0     3662 2023-01-17 09:28:46.411910 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast.py
--rw-r--r--   0        0        0     1540 2023-01-17 09:28:46.314481 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast_rtp_transport_type.py
--rw-r--r--   0        0        0    21919 2023-01-17 09:28:46.896172 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video.py
--rw-r--r--   0        0        0     1453 2023-01-17 09:28:46.326211 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_constant_bit_rate.py
--rw-r--r--   0        0        0     1545 2023-01-17 09:28:46.383474 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_intelligent_info_display_method.py
--rw-r--r--   0        0        0     1438 2023-01-17 09:28:46.349192 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_max_frame_rate.py
--rw-r--r--   0        0        0     1751 2023-01-17 09:28:46.421579 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_smart_codec.py
--rw-r--r--   0        0        0     1978 2023-01-17 09:28:46.476978 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_svc.py
--rw-r--r--   0        0        0     1433 2023-01-17 09:28:46.402858 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_lower_cap.py
--rw-r--r--   0        0        0     1433 2023-01-17 09:28:46.434992 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_upper_cap.py
--rw-r--r--   0        0        0     1448 2023-01-17 09:28:46.429461 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_codec_type.py
--rw-r--r--   0        0        0     1476 2023-01-17 09:28:46.419483 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_input_channel_id.py
--rw-r--r--   0        0        0     1496 2023-01-17 09:28:46.442880 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_quality_control_type.py
--rw-r--r--   0        0        0     1483 2023-01-17 09:28:46.441323 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_height.py
--rw-r--r--   0        0        0     1478 2023-01-17 09:28:46.463402 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_width.py
--rw-r--r--   0        0        0     3211 2023-01-17 09:28:46.515481 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py
--rw-r--r--   0        0        0     3083 2023-01-17 09:28:46.528633 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py
--rw-r--r--   0        0        0     3354 2023-01-17 09:28:46.580823 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py
--rw-r--r--   0        0        0    18177 2023-01-17 09:28:46.889261 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py
--rw-r--r--   0        0        0     4669 2023-01-17 09:28:46.597468 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py
--rw-r--r--   0        0        0     1544 2023-01-17 09:28:46.512766 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py
--rw-r--r--   0        0        0     3644 2023-01-17 09:28:46.585232 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py
--rw-r--r--   0        0        0     1765 2023-01-17 09:28:46.516351 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py
--rw-r--r--   0        0        0     1442 2023-01-17 09:28:46.545356 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py
--rw-r--r--   0        0        0     1482 2023-01-17 09:28:46.548200 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py
--rw-r--r--   0        0        0     1544 2023-01-17 09:28:46.604136 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py
--rw-r--r--   0        0        0     1452 2023-01-17 09:28:46.606871 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py
--rw-r--r--   0        0        0     1411 2023-01-17 09:28:46.583656 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py
--rw-r--r--   0        0        0     1386 2023-01-17 09:28:46.598170 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py
--rw-r--r--   0        0        0     1462 2023-01-17 09:28:46.603126 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py
--rw-r--r--   0        0        0     1452 2023-01-17 09:28:46.596931 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py
--rw-r--r--   0        0        0     1459 2023-01-17 09:28:46.611941 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py
--rw-r--r--   0        0        0     1431 2023-01-17 09:28:46.615124 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py
--rw-r--r--   0        0        0     1444 2023-01-17 09:28:46.671631 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py
--rw-r--r--   0        0        0     2845 2023-01-17 09:28:46.717133 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py
--rw-r--r--   0        0        0     2224 2023-01-17 09:28:46.713714 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py
--rw-r--r--   0        0        0     2558 2023-01-17 09:28:46.720894 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_user_check.py
--rw-r--r--   0        0        0     4455 2023-01-17 09:28:46.783957 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py
--rw-r--r--   0        0        0     2890 2023-01-17 09:28:46.724086 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py
--rw-r--r--   0        0        0     3020 2023-01-17 09:28:46.736237 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py
--rw-r--r--   0        0        0     3281 2023-01-17 09:28:46.746342 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py
--rw-r--r--   0        0        0     9938 2023-01-17 09:28:46.874915 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py
--rw-r--r--   0        0        0     1370 2023-01-17 09:28:46.687064 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py
--rw-r--r--   0        0        0     1408 2023-01-17 09:28:46.696339 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py
--rw-r--r--   0        0        0     1380 2023-01-17 09:28:46.744331 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py
--rw-r--r--   0        0        0     1403 2023-01-17 09:28:46.763242 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py
--rw-r--r--   0        0        0     1398 2023-01-17 09:28:46.764354 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py
--rw-r--r--   0        0        0     1418 2023-01-17 09:28:46.764263 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py
--rw-r--r--   0        0        0     1451 2023-01-17 09:28:46.769601 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py
--rw-r--r--   0        0        0       25 2023-01-17 09:28:41.308137 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/py.typed
--rw-r--r--   0        0        0      974 2023-01-17 09:28:46.760960 hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/types.py
--rw-r--r--   0        0        0      109 2023-01-17 09:14:45.313429 hikvision_isapi_cli-1.0.8/hikvision_isapi_sk/__init__.py
--rw-r--r--   0        0        0     3491 2023-01-17 10:25:44.164784 hikvision_isapi_cli-1.0.8/hikvision_isapi_sk/session.py
--rw-r--r--   0        0        0      897 2023-01-17 10:30:33.037504 hikvision_isapi_cli-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.0.8/setup.py
--rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-17 09:28:38.348946 hikvision_isapi_cli-1.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3768 2023-01-17 09:21:44.810775 hikvision_isapi_cli-1.0.9/README.md
+-rw-r--r--   0        0        0       24 2023-01-17 09:37:47.368937 hikvision_isapi_cli-1.0.9/docs/API.md
+-rw-r--r--   0        0        0      105 2023-01-17 09:28:44.011639 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/__init__.py
+-rw-r--r--   0        0        0       47 2023-01-17 09:28:41.487139 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 09:28:41.561189 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/__init__.py
+-rw-r--r--   0        0        0     3809 2023-01-17 09:28:44.165751 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py
+-rw-r--r--   0        0        0    13745 2023-01-17 09:28:44.205063 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py
+-rw-r--r--   0        0        0     4919 2023-01-17 09:28:44.246344 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py
+-rw-r--r--   0        0        0     3682 2023-01-17 09:28:44.223723 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_heartbeat.py
+-rw-r--r--   0        0        0     7421 2023-01-17 09:28:44.296708 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_login.py
+-rw-r--r--   0        0        0     4609 2023-01-17 10:22:12.718839 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_login_capabilities.py
+-rw-r--r--   0        0        0        0 2023-01-17 09:28:41.505499 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/__init__.py
+-rw-r--r--   0        0        0     4318 2023-01-17 09:28:44.295091 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/callstatus.py
+-rw-r--r--   0        0        0     4624 2023-01-17 09:28:44.310084 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py
+-rw-r--r--   0        0        0     4330 2023-01-17 09:28:44.326899 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilities.py
+-rw-r--r--   0        0        0     2296 2023-01-17 09:28:44.310713 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilities1.py
+-rw-r--r--   0        0        0     2285 2023-01-17 09:28:44.304335 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilties.py
+-rw-r--r--   0        0        0     4379 2023-01-17 09:28:44.386660 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels.py
+-rw-r--r--   0        0        0     2271 2023-01-17 09:28:44.322586 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels2.py
+-rw-r--r--   0        0        0     5421 2023-01-17 09:28:44.464774 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py
+-rw-r--r--   0        0        0     2578 2023-01-17 09:28:44.374131 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py
+-rw-r--r--   0        0        0     4105 2023-01-17 09:28:44.429018 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_close.py
+-rw-r--r--   0        0        0     4150 2023-01-17 09:28:44.420673 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_open.py
+-rw-r--r--   0        0        0     2553 2023-01-17 09:28:44.362666 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_picture.py
+-rw-r--r--   0        0        0     2902 2023-01-17 09:28:44.393953 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py
+-rw-r--r--   0        0        0     2276 2023-01-17 09:28:44.362814 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceid.py
+-rw-r--r--   0        0        0     2341 2023-01-17 09:28:44.369285 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py
+-rw-r--r--   0        0        0     4226 2023-01-17 09:28:44.473777 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceinfo.py
+-rw-r--r--   0        0        0     5497 2023-01-17 09:28:44.507906 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/door.py
+-rw-r--r--   0        0        0     4442 2023-01-17 09:28:44.498441 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/door_capabilities.py
+-rw-r--r--   0        0        0     2853 2023-01-17 09:28:44.466706 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/encryption_format_json.py
+-rw-r--r--   0        0        0     4018 2023-01-17 09:28:44.464150 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py
+-rw-r--r--   0        0        0     2257 2023-01-17 09:28:44.438111 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/index1.py
+-rw-r--r--   0        0        0     4422 2023-01-17 09:28:44.508771 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/inputs_channels.py
+-rw-r--r--   0        0        0     2262 2023-01-17 09:28:44.519160 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/status.py
+-rw-r--r--   0        0        0     3554 2023-01-17 09:28:44.554694 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/usercheck.py
+-rw-r--r--   0        0        0     2506 2023-01-17 09:28:44.513242 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/userpermission1.py
+-rw-r--r--   0        0        0     2256 2023-01-17 09:28:44.506578 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/users.py
+-rw-r--r--   0        0        0     2234 2023-01-17 10:17:26.800994 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/client.py
+-rw-r--r--   0        0        0      282 2023-01-17 09:28:44.413275 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/errors.py
+-rw-r--r--   0        0        0    62059 2023-01-17 09:28:43.126388 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/__init__.py
+-rw-r--r--   0        0        0     2319 2023-01-17 09:28:44.557911 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_call_status.py
+-rw-r--r--   0        0        0     1578 2023-01-17 09:28:44.517380 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py
+-rw-r--r--   0        0        0     2477 2023-01-17 09:28:44.596931 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py
+-rw-r--r--   0        0        0     2388 2023-01-17 09:28:44.620077 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py
+-rw-r--r--   0        0        0     1749 2023-01-17 09:28:44.585989 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py
+-rw-r--r--   0        0        0     4019 2023-01-17 09:28:44.697631 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_response_status.py
+-rw-r--r--   0        0        0     6780 2023-01-17 09:28:44.632655 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py
+-rw-r--r--   0        0        0   165585 2023-01-17 09:28:47.928951 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py
+-rw-r--r--   0        0        0     5642 2023-01-17 09:28:44.719289 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py
+-rw-r--r--   0        0        0     1763 2023-01-17 09:28:44.608416 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py
+-rw-r--r--   0        0        0     1980 2023-01-17 09:28:44.620086 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py
+-rw-r--r--   0        0        0     1526 2023-01-17 09:28:44.585205 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py
+-rw-r--r--   0        0        0     3004 2023-01-17 09:28:44.658442 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py
+-rw-r--r--   0        0        0     1702 2023-01-17 09:28:44.632498 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py
+-rw-r--r--   0        0        0     1416 2023-01-17 09:28:44.603468 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py
+-rw-r--r--   0        0        0     1426 2023-01-17 09:28:44.635169 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py
+-rw-r--r--   0        0        0     1472 2023-01-17 09:28:44.631448 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py
+-rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.661025 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py
+-rw-r--r--   0        0        0     1449 2023-01-17 09:28:44.664678 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1523 2023-01-17 09:28:44.671433 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py
+-rw-r--r--   0        0        0     1494 2023-01-17 09:28:44.672263 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py
+-rw-r--r--   0        0        0     1456 2023-01-17 09:28:44.684836 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py
+-rw-r--r--   0        0        0     1531 2023-01-17 09:28:44.700495 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py
+-rw-r--r--   0        0        0     1531 2023-01-17 09:28:44.704043 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py
+-rw-r--r--   0        0        0     1449 2023-01-17 09:28:44.714058 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py
+-rw-r--r--   0        0        0     1464 2023-01-17 09:28:44.725640 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py
+-rw-r--r--   0        0        0     1441 2023-01-17 09:28:44.726762 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py
+-rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.736164 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py
+-rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.759420 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py
+-rw-r--r--   0        0        0     1484 2023-01-17 09:28:44.768894 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py
+-rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.752142 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py
+-rw-r--r--   0        0        0     1441 2023-01-17 09:28:44.771591 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py
+-rw-r--r--   0        0        0     1456 2023-01-17 09:28:44.755495 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py
+-rw-r--r--   0        0        0     1529 2023-01-17 09:28:44.778762 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.793587 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.794148 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py
+-rw-r--r--   0        0        0     1534 2023-01-17 09:28:44.801996 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1519 2023-01-17 09:28:44.789440 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py
+-rw-r--r--   0        0        0     1561 2023-01-17 09:28:44.790227 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py
+-rw-r--r--   0        0        0     1541 2023-01-17 09:28:44.849609 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py
+-rw-r--r--   0        0        0     1579 2023-01-17 09:28:44.789177 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py
+-rw-r--r--   0        0        0     1489 2023-01-17 09:28:44.816126 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py
+-rw-r--r--   0        0        0     1536 2023-01-17 09:28:44.807582 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.881162 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py
+-rw-r--r--   0        0        0     1477 2023-01-17 09:28:44.843116 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1464 2023-01-17 09:28:44.844215 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py
+-rw-r--r--   0        0        0     1539 2023-01-17 09:28:44.853548 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py
+-rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.892166 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py
+-rw-r--r--   0        0        0     1454 2023-01-17 09:28:44.870941 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py
+-rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.884542 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py
+-rw-r--r--   0        0        0     1461 2023-01-17 09:28:44.919210 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.875298 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py
+-rw-r--r--   0        0        0     1421 2023-01-17 09:28:44.871197 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py
+-rw-r--r--   0        0        0     1544 2023-01-17 09:28:44.896393 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1539 2023-01-17 09:28:44.891937 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:44.907613 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py
+-rw-r--r--   0        0        0     1526 2023-01-17 09:28:44.945100 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py
+-rw-r--r--   0        0        0     1524 2023-01-17 09:28:44.952479 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py
+-rw-r--r--   0        0        0     1487 2023-01-17 09:28:44.953669 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py
+-rw-r--r--   0        0        0     1467 2023-01-17 09:28:44.927748 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py
+-rw-r--r--   0        0        0     1489 2023-01-17 09:28:44.968629 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py
+-rw-r--r--   0        0        0     1474 2023-01-17 09:28:44.976680 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.013844 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py
+-rw-r--r--   0        0        0     1474 2023-01-17 09:28:44.997502 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py
+-rw-r--r--   0        0        0     1467 2023-01-17 09:28:45.001387 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py
+-rw-r--r--   0        0        0     1449 2023-01-17 09:28:45.000540 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py
+-rw-r--r--   0        0        0     1526 2023-01-17 09:28:45.008879 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py
+-rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.003127 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py
+-rw-r--r--   0        0        0     1426 2023-01-17 09:28:44.985372 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py
+-rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.015304 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py
+-rw-r--r--   0        0        0     1479 2023-01-17 09:28:44.992737 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py
+-rw-r--r--   0        0        0     1439 2023-01-17 09:28:45.021871 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py
+-rw-r--r--   0        0        0     1472 2023-01-17 09:28:45.035228 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py
+-rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.065123 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py
+-rw-r--r--   0        0        0     1449 2023-01-17 09:28:45.058724 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py
+-rw-r--r--   0        0        0     1524 2023-01-17 09:28:45.062420 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py
+-rw-r--r--   0        0        0     1456 2023-01-17 09:28:45.084556 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py
+-rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.113704 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py
+-rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.091358 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py
+-rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.108179 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py
+-rw-r--r--   0        0        0     1477 2023-01-17 09:28:45.104285 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py
+-rw-r--r--   0        0        0     1469 2023-01-17 09:28:45.069155 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py
+-rw-r--r--   0        0        0     1484 2023-01-17 09:28:45.079718 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py
+-rw-r--r--   0        0        0     1474 2023-01-17 09:28:45.133736 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py
+-rw-r--r--   0        0        0     1482 2023-01-17 09:28:45.096529 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py
+-rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.131052 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py
+-rw-r--r--   0        0        0     1489 2023-01-17 09:28:45.126681 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py
+-rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.155690 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py
+-rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.136752 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py
+-rw-r--r--   0        0        0     1469 2023-01-17 09:28:45.162768 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py
+-rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.159455 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py
+-rw-r--r--   0        0        0     1464 2023-01-17 09:28:45.179237 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py
+-rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.182935 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py
+-rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.178892 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py
+-rw-r--r--   0        0        0     1474 2023-01-17 09:28:45.185641 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py
+-rw-r--r--   0        0        0     1484 2023-01-17 09:28:45.195403 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py
+-rw-r--r--   0        0        0     1431 2023-01-17 09:28:45.198666 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py
+-rw-r--r--   0        0        0     1539 2023-01-17 09:28:45.217864 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.222882 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py
+-rw-r--r--   0        0        0     1521 2023-01-17 09:28:45.222515 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.224729 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1479 2023-01-17 09:28:45.229810 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py
+-rw-r--r--   0        0        0     1477 2023-01-17 09:28:45.215842 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py
+-rw-r--r--   0        0        0     1436 2023-01-17 09:28:45.230514 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.236376 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py
+-rw-r--r--   0        0        0     1446 2023-01-17 09:28:45.250607 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py
+-rw-r--r--   0        0        0     5455 2023-01-17 09:28:45.366437 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py
+-rw-r--r--   0        0        0     1604 2023-01-17 09:28:45.255042 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py
+-rw-r--r--   0        0        0     1599 2023-01-17 09:28:45.266895 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py
+-rw-r--r--   0        0        0     3009 2023-01-17 09:28:45.312915 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py
+-rw-r--r--   0        0        0     5227 2023-01-17 09:28:45.437027 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py
+-rw-r--r--   0        0        0     1677 2023-01-17 09:28:45.293200 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py
+-rw-r--r--   0        0        0     1927 2023-01-17 09:28:45.332567 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py
+-rw-r--r--   0        0        0     1934 2023-01-17 09:28:45.323033 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py
+-rw-r--r--   0        0        0     4548 2023-01-17 09:28:45.344849 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info.py
+-rw-r--r--   0        0        0    31772 2023-01-17 09:28:46.707479 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py
+-rw-r--r--   0        0        0    12689 2023-01-17 09:28:45.680285 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py
+-rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.309553 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py
+-rw-r--r--   0        0        0     1464 2023-01-17 09:28:45.308839 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:45.325592 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py
+-rw-r--r--   0        0        0     1461 2023-01-17 09:28:45.325605 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py
+-rw-r--r--   0        0        0     1466 2023-01-17 09:28:45.338781 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py
+-rw-r--r--   0        0        0     1492 2023-01-17 09:28:45.352163 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py
+-rw-r--r--   0        0        0     1451 2023-01-17 09:28:45.366644 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py
+-rw-r--r--   0        0        0     1526 2023-01-17 09:28:45.380821 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py
+-rw-r--r--   0        0        0     3040 2023-01-17 09:28:45.457977 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py
+-rw-r--r--   0        0        0     2645 2023-01-17 09:28:45.479705 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py
+-rw-r--r--   0        0        0     1695 2023-01-17 09:28:45.397415 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py
+-rw-r--r--   0        0        0     1848 2023-01-17 09:28:45.440252 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py
+-rw-r--r--   0        0        0     1848 2023-01-17 09:28:45.434439 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py
+-rw-r--r--   0        0        0     1706 2023-01-17 09:28:45.431562 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py
+-rw-r--r--   0        0        0     1871 2023-01-17 09:28:45.456354 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py
+-rw-r--r--   0        0        0     3132 2023-01-17 09:28:45.492249 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py
+-rw-r--r--   0        0        0     2953 2023-01-17 09:28:45.478352 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py
+-rw-r--r--   0        0        0     3208 2023-01-17 09:28:45.544013 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py
+-rw-r--r--   0        0        0     7425 2023-01-17 09:28:45.735354 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py
+-rw-r--r--   0        0        0     4767 2023-01-17 09:28:45.609815 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py
+-rw-r--r--   0        0        0     1961 2023-01-17 09:28:45.544461 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py
+-rw-r--r--   0        0        0     1752 2023-01-17 09:28:45.529158 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py
+-rw-r--r--   0        0        0     3140 2023-01-17 09:28:45.603716 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py
+-rw-r--r--   0        0        0     2544 2023-01-17 09:28:45.578190 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py
+-rw-r--r--   0        0        0     1913 2023-01-17 09:28:45.564143 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py
+-rw-r--r--   0        0        0     2803 2023-01-17 09:28:45.606574 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py
+-rw-r--r--   0        0        0     2400 2023-01-17 09:28:45.609354 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py
+-rw-r--r--   0        0        0     2690 2023-01-17 09:28:45.613220 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status.py
+-rw-r--r--   0        0        0     2997 2023-01-17 09:28:45.624642 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py
+-rw-r--r--   0        0        0     4161 2023-01-17 09:28:45.729227 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py
+-rw-r--r--   0        0        0     3141 2023-01-17 09:28:45.708994 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py
+-rw-r--r--   0        0        0     2719 2023-01-17 09:28:45.677094 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login.py
+-rw-r--r--   0        0        0     2958 2023-01-17 09:28:45.685381 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py
+-rw-r--r--   0        0        0     3693 2023-01-17 09:28:45.767088 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py
+-rw-r--r--   0        0        0     2746 2023-01-17 09:28:45.714580 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py
+-rw-r--r--   0        0        0     3581 2023-01-17 09:28:45.772521 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py
+-rw-r--r--   0        0        0     3971 2023-01-17 09:28:45.798419 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py
+-rw-r--r--   0        0        0     6459 2023-01-17 09:28:45.735364 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py
+-rw-r--r--   0        0        0     2966 2023-01-17 09:28:45.745494 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py
+-rw-r--r--   0        0        0     7988 2023-01-17 09:28:45.990228 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel.py
+-rw-r--r--   0        0        0     7796 2023-01-17 09:28:45.912701 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio.py
+-rw-r--r--   0        0        0     1478 2023-01-17 09:28:45.730947 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_compression_type.py
+-rw-r--r--   0        0        0     1540 2023-01-17 09:28:45.750745 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_inbound_compression_type.py
+-rw-r--r--   0        0        0     1995 2023-01-17 09:28:45.786244 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_voice_changer.py
+-rw-r--r--   0        0        0     3132 2023-01-17 09:28:45.820585 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable.py
+-rw-r--r--   0        0        0     8197 2023-01-17 09:28:46.107125 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel.py
+-rw-r--r--   0        0        0     8968 2023-01-17 09:28:46.125763 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio.py
+-rw-r--r--   0        0        0     1722 2023-01-17 09:28:45.810634 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_compression_type.py
+-rw-r--r--   0        0        0     1760 2023-01-17 09:28:45.813507 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_inbound_compression_type.py
+-rw-r--r--   0        0        0     2210 2023-01-17 09:28:45.847710 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_voice_changer.py
+-rw-r--r--   0        0        0    12227 2023-01-17 09:28:46.276001 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport.py
+-rw-r--r--   0        0        0     3726 2023-01-17 09:28:45.905456 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list.py
+-rw-r--r--   0        0        0     4009 2023-01-17 09:28:45.886817 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol.py
+-rw-r--r--   0        0        0     1914 2023-01-17 09:28:45.858021 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py
+-rw-r--r--   0        0        0     8096 2023-01-17 09:28:46.159775 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast.py
+-rw-r--r--   0        0        0     1800 2023-01-17 09:28:45.878574 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_active_multicast_enabled.py
+-rw-r--r--   0        0        0     5373 2023-01-17 09:28:46.084313 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info.py
+-rw-r--r--   0        0        0     1799 2023-01-17 09:28:45.910566 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py
+-rw-r--r--   0        0        0     1768 2023-01-17 09:28:45.913968 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_ratio.py
+-rw-r--r--   0        0        0     4229 2023-01-17 09:28:46.096223 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security.py
+-rw-r--r--   0        0        0     2144 2023-01-17 09:28:45.979100 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security_security_algorithm.py
+-rw-r--r--   0        0        0     2593 2023-01-17 09:28:46.060572 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_srtp_multicast.py
+-rw-r--r--   0        0        0     4164 2023-01-17 09:28:46.137367 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast.py
+-rw-r--r--   0        0        0     1760 2023-01-17 09:28:46.026195 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast_rtp_transport_type.py
+-rw-r--r--   0        0        0    26045 2023-01-17 09:28:46.811142 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video.py
+-rw-r--r--   0        0        0     1692 2023-01-17 09:28:45.994255 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_constant_bit_rate.py
+-rw-r--r--   0        0        0     1765 2023-01-17 09:28:45.999781 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_intelligent_info_display_method.py
+-rw-r--r--   0        0        0     1677 2023-01-17 09:28:46.114782 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_max_frame_rate.py
+-rw-r--r--   0        0        0     1966 2023-01-17 09:28:46.165568 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_smart_codec.py
+-rw-r--r--   0        0        0     2187 2023-01-17 09:28:46.184574 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_svc.py
+-rw-r--r--   0        0        0     1672 2023-01-17 09:28:46.126741 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_lower_cap.py
+-rw-r--r--   0        0        0     1672 2023-01-17 09:28:46.142200 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_upper_cap.py
+-rw-r--r--   0        0        0     1687 2023-01-17 09:28:46.170829 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_codec_type.py
+-rw-r--r--   0        0        0     1720 2023-01-17 09:28:46.171237 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_input_channel_id.py
+-rw-r--r--   0        0        0     1740 2023-01-17 09:28:46.179507 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_quality_control_type.py
+-rw-r--r--   0        0        0     1727 2023-01-17 09:28:46.194620 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_height.py
+-rw-r--r--   0        0        0     1722 2023-01-17 09:28:46.237142 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_width.py
+-rw-r--r--   0        0        0    10309 2023-01-17 09:28:46.511602 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport.py
+-rw-r--r--   0        0        0     3241 2023-01-17 09:28:46.259865 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list.py
+-rw-r--r--   0        0        0     3530 2023-01-17 09:28:46.328623 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol.py
+-rw-r--r--   0        0        0     1729 2023-01-17 09:28:46.217905 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py
+-rw-r--r--   0        0        0     7234 2023-01-17 09:28:46.516345 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast.py
+-rw-r--r--   0        0        0     1580 2023-01-17 09:28:46.232355 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_active_multicast_enabled.py
+-rw-r--r--   0        0        0     4535 2023-01-17 09:28:46.352913 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info.py
+-rw-r--r--   0        0        0     1579 2023-01-17 09:28:46.258633 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py
+-rw-r--r--   0        0        0     1548 2023-01-17 09:28:46.268360 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_ratio.py
+-rw-r--r--   0        0        0     3749 2023-01-17 09:28:46.373824 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security.py
+-rw-r--r--   0        0        0     1948 2023-01-17 09:28:46.371111 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security_security_algorithm.py
+-rw-r--r--   0        0        0     2378 2023-01-17 09:28:46.335273 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_srtp_multicast.py
+-rw-r--r--   0        0        0     3662 2023-01-17 09:28:46.411910 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast.py
+-rw-r--r--   0        0        0     1540 2023-01-17 09:28:46.314481 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast_rtp_transport_type.py
+-rw-r--r--   0        0        0    21919 2023-01-17 09:28:46.896172 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video.py
+-rw-r--r--   0        0        0     1453 2023-01-17 09:28:46.326211 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_constant_bit_rate.py
+-rw-r--r--   0        0        0     1545 2023-01-17 09:28:46.383474 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_intelligent_info_display_method.py
+-rw-r--r--   0        0        0     1438 2023-01-17 09:28:46.349192 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_max_frame_rate.py
+-rw-r--r--   0        0        0     1751 2023-01-17 09:28:46.421579 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_smart_codec.py
+-rw-r--r--   0        0        0     1978 2023-01-17 09:28:46.476978 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_svc.py
+-rw-r--r--   0        0        0     1433 2023-01-17 09:28:46.402858 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_lower_cap.py
+-rw-r--r--   0        0        0     1433 2023-01-17 09:28:46.434992 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_upper_cap.py
+-rw-r--r--   0        0        0     1448 2023-01-17 09:28:46.429461 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_codec_type.py
+-rw-r--r--   0        0        0     1476 2023-01-17 09:28:46.419483 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_input_channel_id.py
+-rw-r--r--   0        0        0     1496 2023-01-17 09:28:46.442880 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_quality_control_type.py
+-rw-r--r--   0        0        0     1483 2023-01-17 09:28:46.441323 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_height.py
+-rw-r--r--   0        0        0     1478 2023-01-17 09:28:46.463402 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_width.py
+-rw-r--r--   0        0        0     3211 2023-01-17 09:28:46.515481 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py
+-rw-r--r--   0        0        0     3083 2023-01-17 09:28:46.528633 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py
+-rw-r--r--   0        0        0     3354 2023-01-17 09:28:46.580823 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py
+-rw-r--r--   0        0        0    18177 2023-01-17 09:28:46.889261 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py
+-rw-r--r--   0        0        0     4669 2023-01-17 09:28:46.597468 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py
+-rw-r--r--   0        0        0     1544 2023-01-17 09:28:46.512766 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py
+-rw-r--r--   0        0        0     3644 2023-01-17 09:28:46.585232 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py
+-rw-r--r--   0        0        0     1765 2023-01-17 09:28:46.516351 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py
+-rw-r--r--   0        0        0     1442 2023-01-17 09:28:46.545356 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py
+-rw-r--r--   0        0        0     1482 2023-01-17 09:28:46.548200 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py
+-rw-r--r--   0        0        0     1544 2023-01-17 09:28:46.604136 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py
+-rw-r--r--   0        0        0     1452 2023-01-17 09:28:46.606871 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py
+-rw-r--r--   0        0        0     1411 2023-01-17 09:28:46.583656 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py
+-rw-r--r--   0        0        0     1386 2023-01-17 09:28:46.598170 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py
+-rw-r--r--   0        0        0     1462 2023-01-17 09:28:46.603126 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py
+-rw-r--r--   0        0        0     1452 2023-01-17 09:28:46.596931 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py
+-rw-r--r--   0        0        0     1459 2023-01-17 09:28:46.611941 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py
+-rw-r--r--   0        0        0     1431 2023-01-17 09:28:46.615124 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py
+-rw-r--r--   0        0        0     1444 2023-01-17 09:28:46.671631 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py
+-rw-r--r--   0        0        0     2845 2023-01-17 09:28:46.717133 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py
+-rw-r--r--   0        0        0     2224 2023-01-17 09:28:46.713714 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py
+-rw-r--r--   0        0        0     2558 2023-01-17 09:28:46.720894 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_user_check.py
+-rw-r--r--   0        0        0     4455 2023-01-17 09:28:46.783957 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py
+-rw-r--r--   0        0        0     2890 2023-01-17 09:28:46.724086 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py
+-rw-r--r--   0        0        0     3020 2023-01-17 09:28:46.736237 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py
+-rw-r--r--   0        0        0     3281 2023-01-17 09:28:46.746342 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py
+-rw-r--r--   0        0        0     9938 2023-01-17 09:28:46.874915 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py
+-rw-r--r--   0        0        0     1370 2023-01-17 09:28:46.687064 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py
+-rw-r--r--   0        0        0     1408 2023-01-17 09:28:46.696339 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py
+-rw-r--r--   0        0        0     1380 2023-01-17 09:28:46.744331 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py
+-rw-r--r--   0        0        0     1403 2023-01-17 09:28:46.763242 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py
+-rw-r--r--   0        0        0     1398 2023-01-17 09:28:46.764354 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py
+-rw-r--r--   0        0        0     1418 2023-01-17 09:28:46.764263 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py
+-rw-r--r--   0        0        0     1451 2023-01-17 09:28:46.769601 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py
+-rw-r--r--   0        0        0       25 2023-01-17 09:28:41.308137 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/py.typed
+-rw-r--r--   0        0        0      974 2023-01-17 09:28:46.760960 hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/types.py
+-rw-r--r--   0        0        0      109 2023-01-17 09:14:45.313429 hikvision_isapi_cli-1.0.9/hikvision_isapi_sk/__init__.py
+-rw-r--r--   0        0        0     3806 2023-01-17 13:05:00.895815 hikvision_isapi_cli-1.0.9/hikvision_isapi_sk/session.py
+-rw-r--r--   0        0        0      897 2023-01-17 13:01:26.164502 hikvision_isapi_cli-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.0.9/setup.py
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.0.9/PKG-INFO
```

### Comparing `hikvision_isapi_cli-1.0.8/README.md` & `hikvision_isapi_cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_heartbeat.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_heartbeat.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_login.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/default/session_login_capabilities.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/default/session_login_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/callstatus.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/callstatus.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilities.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilities1.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilities1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/capabilties.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/capabilties.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels2.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels2.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_close.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_close.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_open.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_open.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/channels_1_picture.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/channels_1_picture.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceid.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceid.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/deviceinfo.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/door_capabilities.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/door_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/encryption_format_json.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/encryption_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/index1.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/index1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/inputs_channels.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/inputs_channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/usercheck.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/usercheck.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/userpermission1.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/userpermission1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/api/isapi/users.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/api/isapi/users.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/client.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/client.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/__init__.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_call_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_json_response_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_json_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_inbound_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_audio_inbound_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_voice_changer.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_audio_voice_changer.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_inbound_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_audio_inbound_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_voice_changer.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_audio_voice_changer.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_active_multicast_enabled.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_active_multicast_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_ratio.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_multicast_fec_info_fec_ratio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security_security_algorithm.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_security_security_algorithm.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_srtp_multicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_srtp_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast_rtp_transport_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_transport_unicast_rtp_transport_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_constant_bit_rate.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_constant_bit_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_intelligent_info_display_method.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_intelligent_info_display_method.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_max_frame_rate.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_max_frame_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_smart_codec.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_smart_codec.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_svc.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_svc.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_lower_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_lower_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_upper_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_vbr_upper_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_codec_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_codec_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_input_channel_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_quality_control_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_quality_control_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_height.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_height.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_width.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_custom_stream_enable_streaming_channel_video_video_resolution_width.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_control_protocol_list_control_protocol_streaming_transport.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_active_multicast_enabled.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_active_multicast_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_dest_port_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_ratio.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_multicast_fec_info_fec_ratio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security_security_algorithm.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_security_security_algorithm.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_srtp_multicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_srtp_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast_rtp_transport_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_transport_unicast_rtp_transport_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_constant_bit_rate.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_constant_bit_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_intelligent_info_display_method.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_intelligent_info_display_method.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_max_frame_rate.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_max_frame_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_smart_codec.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_smart_codec.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_svc.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_svc.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_lower_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_lower_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_upper_cap.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_vbr_upper_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_codec_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_codec_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_input_channel_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_quality_control_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_quality_control_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_height.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_height.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_width.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_streaming_channel_video_video_resolution_width.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_user_check.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_user_check.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_cli/types.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_cli/types.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.0.8/hikvision_isapi_sk/session.py` & `hikvision_isapi_cli-1.0.9/hikvision_isapi_sk/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,21 +66,29 @@
         login.session_login.is_session_id_valid_long_term = False
         login.session_login.session_id_version = 2
 
         response: Response = session_login.sync_detailed(client=self.client, time_stamp=millis, json_body=login)
         cookies = response.headers["set-cookie"]
         web_session = cookies.split(";")[0].split("=")
 
-        self.client._api.cookies = {web_session[0]: web_session[1]}
+        self.client.cookies = {web_session[0]: web_session[1]}
+        self.client._api.cookies = self.client.cookies
         self.client._asyncio_api.cookies = self.client._api.cookies
 
         response: Response = session_heartbeat.sync_detailed(client=self.client)
         if response.status_code == HTTPStatus.OK:
             return True
         
         _LOGGER.error(response)
         return False
 
     def stop(self) -> None:
         _LOGGER.info("Stop Web Session: " + str(self.client._api.cookies))
+        self.client.cookies={}
         self.client._api.cookies={}
         self.client._asyncio_api.cookies={}
+        
+    async def heartbeat(self) -> bool:
+        response : Response = await session_heartbeat.asyncio_detailed(client=self.client)
+        if response.status_code == HTTPStatus.OK:
+            return True
+        return False
```

### Comparing `hikvision_isapi_cli-1.0.8/pyproject.toml` & `hikvision_isapi_cli-1.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikvision-isapi-cli"
-version = "1.0.8"
+version = "1.0.9"
 description = "A client library for accessing Hikvision ISAPI"
 
 authors = ["mmascia"]
 
 readme = "README.md"
 packages = [
     {include = "hikvision_isapi_cli"},
```

### Comparing `hikvision_isapi_cli-1.0.8/setup.py` & `hikvision_isapi_cli-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest-socket>=0.5.1',
  'pytest>=7.2.0',
  'python-dateutil>=2.8.0,<3.0.0',
  'xmltodict>=0.13.0']
 
 setup_kwargs = {
     'name': 'hikvision-isapi-cli',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'A client library for accessing Hikvision ISAPI',
     'long_description': '# hikvision-isapi-cli\nA client library for accessing Hikvision ISAPI\n\n### OpenAPI Generator\n\n```bash\nrm -fr .history/;cd ..;openapi-python-client update --path hikvision-isapi-cli/openapi.json --custom-template-path=hikvision-isapi-cli/templates/ --config=hikvision-isapi-cli/.config.yaml;cd hikvision-isapi-cli\n```\n\n## Usage\nFirst, create a client:\n\n```python\nfrom hikvision_isapi_cli import Client\n\nclient = Client(base_url="https://api.example.com", username="username", password="SuperSecretPassword")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom hikvision_isapi_cli.models import MyDataModel\nfrom hikvision_isapi_cli.api.my_tag import get_my_data_model\nfrom hikvision_isapi_cli.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom hikvision_isapi_cli.models import MyDataModel\nfrom hikvision_isapi_cli.api.my_tag import get_my_data_model\nfrom hikvision_isapi_cli.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = Client(\n    base_url="https://internal_api.example.com", \n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = Client(\n    base_url="https://internal_api.example.com",  \n    verify_ssl=False\n)\n```\n\nThere are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info.\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `hikvision_isapi_cli.api.default`\n\n## Building / publishing this Client\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:\n1. Update the metadata in pyproject.toml (e.g. authors, version)\n1. If you\'re using a private repository, configure it with Poetry\n    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`\n    1. `poetry config http-basic.<your-repository-name> <username> <password>`\n1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`\n\nIf you want to install this client into another project without publishing it (e.g. for development) then:\n1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project\n1. If that project is not using Poetry:\n    1. Build a wheel with `poetry build -f wheel`\n    1. Install that wheel from the other project `pip install <path-to-wheel>`\n',
     'author': 'mmascia',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hikvision_isapi_cli-1.0.8/PKG-INFO` & `hikvision_isapi_cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikvision-isapi-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client library for accessing Hikvision ISAPI
 Author: mmascia
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.15.4,<0.24.0)
```


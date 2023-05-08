# Comparing `tmp/kittycad-0.4.0.tar.gz` & `tmp/kittycad-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.4.0.tar", max compression
+gzip compressed data, was "kittycad-0.4.1.tar", max compression
```

## Comparing `kittycad-0.4.0.tar` & `kittycad-0.4.1.tar`

### file list

```diff
@@ -1,271 +1,271 @@
--rw-r--r--   0        0        0     1065 2023-05-08 20:06:09.479519 kittycad-0.4.0/LICENSE
--rw-r--r--   0        0        0      875 2023-05-08 20:06:09.479519 kittycad-0.4.0/README.md
--rw-r--r--   0        0        0       48 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3781 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3559 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3110 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2799 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3243 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6149 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4236 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     5005 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4815 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4351 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2879 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2784 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4284 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2911 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2338 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      142 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/__init__.py
--rw-r--r--   0        0        0     2786 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/cmd.py
--rw-r--r--   0        0        0     2684 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/cmd_batch.py
--rw-r--r--   0        0        0      161 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1781 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3195 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     3871 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4461 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     4276 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     4294 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3855 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3785 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3220 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2139 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2383 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2629 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2564 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2193 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2245 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      123 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2956 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2638 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2431 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2655 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2681 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2616 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2684 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2954 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2483 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3966 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3784 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     4051 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3758 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     4082 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     4230 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3971 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3918 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3955 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3848 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3886 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3919 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2757 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3061 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3185 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2480 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2506 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2523 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2629 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4105 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4187 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2779 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/client.py
--rw-r--r--   0        0        0     5250 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/client_test.py
--rw-r--r--   0        0        0   127516 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/examples_test.py
--rw-r--r--   0        0        0     7838 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8266 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3278 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5747 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34040 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/customer.py
--rw-r--r--   0        0        0     4306 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     3553 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd.py
--rw-r--r--   0        0        0       75 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_id.py
--rw-r--r--   0        0        0     2441 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_req.py
--rw-r--r--   0        0        0     1746 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_req_batch.py
--rw-r--r--   0        0        0     2393 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_error.py
--rw-r--r--   0        0        0     1869 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_outcome.py
--rw-r--r--   0        0        0     1505 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_outcomes.py
--rw-r--r--   0        0        0     1789 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      269 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     5700 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6060 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5725 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5707 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5522 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5428 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1337 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/method.py
--rw-r--r--   0        0        0     3081 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2501 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5424 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1498 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3638 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6317 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      642 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      916 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6360 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      754 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      888 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      380 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6330 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      752 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      539 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6377 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      656 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6252 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0     1488 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0     1162 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      645 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6304 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      584 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     2187 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6442 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      402 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6321 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      389 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1094 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0     3438 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6259 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6287 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6297 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      468 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6265 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      725 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6278 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      586 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6330 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      570 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6295 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      500 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6304 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      674 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      902 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6265 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      753 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6252 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      452 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     3286 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2577 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/types.py
--rw-r--r--   0        0        0     2472 2023-05-08 20:06:09.911528 kittycad-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-08 21:32:05.549300 kittycad-0.4.1/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-08 21:32:05.549300 kittycad-0.4.1/README.md
+-rw-r--r--   0        0        0       48 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3781 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3559 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3110 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2799 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3243 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6149 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4236 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5005 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4815 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4351 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2879 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2784 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4284 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2911 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2338 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      142 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/__init__.py
+-rw-r--r--   0        0        0     2786 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/cmd.py
+-rw-r--r--   0        0        0     2684 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/cmd_batch.py
+-rw-r--r--   0        0        0      161 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1781 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3195 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     3871 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4461 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     4276 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     4294 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3855 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3785 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3220 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2139 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2383 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2629 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2564 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2193 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2245 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      123 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2956 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2638 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2431 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2655 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2681 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2616 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2684 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2954 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2483 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3966 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3784 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     4051 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3758 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     4082 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     4230 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3971 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3918 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3955 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3848 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3886 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3919 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2757 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3061 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3185 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2480 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2506 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2523 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2629 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4105 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4187 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2779 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/client.py
+-rw-r--r--   0        0        0     5250 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/client_test.py
+-rw-r--r--   0        0        0   127516 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/examples_test.py
+-rw-r--r--   0        0        0     7838 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8266 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3278 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5747 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34040 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4306 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     3553 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd.py
+-rw-r--r--   0        0        0       75 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_id.py
+-rw-r--r--   0        0        0     2441 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_req.py
+-rw-r--r--   0        0        0     1746 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_req_batch.py
+-rw-r--r--   0        0        0     2393 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_error.py
+-rw-r--r--   0        0        0     1869 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_outcome.py
+-rw-r--r--   0        0        0     1505 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_outcomes.py
+-rw-r--r--   0        0        0     1789 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      269 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     5700 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6060 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5725 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5707 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5522 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5428 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1337 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/method.py
+-rw-r--r--   0        0        0     3081 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2501 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5424 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1498 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3638 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6317 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      642 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6360 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      754 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      888 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      380 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6330 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      752 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      539 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6377 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      656 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6252 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0     1488 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0     1162 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      645 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6304 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      584 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     2187 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6442 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      402 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6321 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      389 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1094 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0     3438 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6259 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6287 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6297 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      468 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6265 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      725 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6278 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      586 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6330 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      570 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6295 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      500 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6304 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      674 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      902 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6265 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      753 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6252 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      452 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     3286 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2577 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/types.py
+-rw-r--r--   0        0        0     2472 2023-05-08 21:32:06.313308 kittycad-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.1/PKG-INFO
```

### Comparing `kittycad-0.4.0/LICENSE` & `kittycad-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/README.md` & `kittycad-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.1/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.1/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.1/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.1/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.1/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.1/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.1/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.1/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.1/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.1/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.1/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.1/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.1/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.1/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.1/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.1/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.1/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.1/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/drawing/cmd.py` & `kittycad-0.4.1/kittycad/api/drawing/cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/drawing/cmd_batch.py` & `kittycad-0.4.1/kittycad/api/drawing/cmd_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.1/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.1/kittycad/api/executor/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.1/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.1/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.1/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_density.py` & `kittycad-0.4.1/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_mass.py` & `kittycad-0.4.1/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.1/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/create_file_volume.py` & `kittycad-0.4.1/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.1/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.1/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.1/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/hidden/logout.py` & `kittycad-0.4.1/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.1/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.1/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.1/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/meta/get_schema.py` & `kittycad-0.4.1/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/meta/ping.py` & `kittycad-0.4.1/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.1/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_time_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_voltage_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.4.1/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.1/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.1/kittycad/api/users/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user.py` & `kittycad-0.4.1/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.1/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.1/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.4.1/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user_self.py` & `kittycad-0.4.1/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.4.1/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/list_users.py` & `kittycad-0.4.1/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/list_users_extended.py` & `kittycad-0.4.1/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/api/users/update_user_self.py` & `kittycad-0.4.1/kittycad/api/users/update_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/client.py` & `kittycad-0.4.1/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/client_test.py` & `kittycad-0.4.1/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/examples_test.py` & `kittycad-0.4.1/kittycad/examples_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/__init__.py` & `kittycad-0.4.1/kittycad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.1/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.1/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.1/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_call_query_group.py` & `kittycad-0.4.1/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.1/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_call_status.py` & `kittycad-0.4.1/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_call_with_price.py` & `kittycad-0.4.1/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.1/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_token.py` & `kittycad-0.4.1/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/api_token_results_page.py` & `kittycad-0.4.1/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/app_client_info.py` & `kittycad-0.4.1/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/async_api_call.py` & `kittycad-0.4.1/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/async_api_call_output.py` & `kittycad-0.4.1/kittycad/models/async_api_call_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.1/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/async_api_call_type.py` & `kittycad-0.4.1/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/billing_info.py` & `kittycad-0.4.1/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/cache_metadata.py` & `kittycad-0.4.1/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/card_details.py` & `kittycad-0.4.1/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/cluster.py` & `kittycad-0.4.1/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/code_output.py` & `kittycad-0.4.1/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/commit.py` & `kittycad-0.4.1/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/connection.py` & `kittycad-0.4.1/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/country_code.py` & `kittycad-0.4.1/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/currency.py` & `kittycad-0.4.1/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/customer.py` & `kittycad-0.4.1/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/customer_balance.py` & `kittycad-0.4.1/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.1/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.1/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.1/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/docker_system_info.py` & `kittycad-0.4.1/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_cmd.py` & `kittycad-0.4.1/kittycad/models/drawing_cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_cmd_req.py` & `kittycad-0.4.1/kittycad/models/drawing_cmd_req.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_cmd_req_batch.py` & `kittycad-0.4.1/kittycad/models/drawing_cmd_req_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_error.py` & `kittycad-0.4.1/kittycad/models/drawing_error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_outcome.py` & `kittycad-0.4.1/kittycad/models/drawing_outcome.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/drawing_outcomes.py` & `kittycad-0.4.1/kittycad/models/drawing_outcomes.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/email_authentication_form.py` & `kittycad-0.4.1/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/engine_metadata.py` & `kittycad-0.4.1/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/error.py` & `kittycad-0.4.1/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/executor_metadata.py` & `kittycad-0.4.1/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/extended_user.py` & `kittycad-0.4.1/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.1/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.1/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_conversion.py` & `kittycad-0.4.1/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_density.py` & `kittycad-0.4.1/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_export_format.py` & `kittycad-0.4.1/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_import_format.py` & `kittycad-0.4.1/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_mass.py` & `kittycad-0.4.1/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_surface_area.py` & `kittycad-0.4.1/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_system_metadata.py` & `kittycad-0.4.1/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/file_volume.py` & `kittycad-0.4.1/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/gateway.py` & `kittycad-0.4.1/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/index_info.py` & `kittycad-0.4.1/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/invoice.py` & `kittycad-0.4.1/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/invoice_line_item.py` & `kittycad-0.4.1/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/invoice_status.py` & `kittycad-0.4.1/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/jetstream.py` & `kittycad-0.4.1/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.1/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/jetstream_config.py` & `kittycad-0.4.1/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/jetstream_stats.py` & `kittycad-0.4.1/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/leaf_node.py` & `kittycad-0.4.1/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/mesh.py` & `kittycad-0.4.1/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.1/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/metadata.py` & `kittycad-0.4.1/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/method.py` & `kittycad-0.4.1/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/new_address.py` & `kittycad-0.4.1/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.1/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/onboarding.py` & `kittycad-0.4.1/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/output_file.py` & `kittycad-0.4.1/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/payment_intent.py` & `kittycad-0.4.1/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/payment_method.py` & `kittycad-0.4.1/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.1/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/physics_constant.py` & `kittycad-0.4.1/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/physics_constant_name.py` & `kittycad-0.4.1/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/plugins_info.py` & `kittycad-0.4.1/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/point_e_metadata.py` & `kittycad-0.4.1/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/pong.py` & `kittycad-0.4.1/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/registry_service_config.py` & `kittycad-0.4.1/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/runtime.py` & `kittycad-0.4.1/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/session.py` & `kittycad-0.4.1/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.1/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_acceleration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_acceleration_format.py` & `kittycad-0.4.1/kittycad/models/unit_acceleration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_angle_format.py` & `kittycad-0.4.1/kittycad/models/unit_angle_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_angular_velocity_format.py` & `kittycad-0.4.1/kittycad/models/unit_angular_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_area_format.py` & `kittycad-0.4.1/kittycad/models/unit_area_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_charge_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_charge_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_concentration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_concentration_format.py` & `kittycad-0.4.1/kittycad/models/unit_concentration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_data_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_data_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_data_format.py` & `kittycad-0.4.1/kittycad/models/unit_data_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_format.py` & `kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_density_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_density_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_density_format.py` & `kittycad-0.4.1/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_energy_format.py` & `kittycad-0.4.1/kittycad/models/unit_energy_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_force_format.py` & `kittycad-0.4.1/kittycad/models/unit_force_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_illuminance_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_illuminance_format.py` & `kittycad-0.4.1/kittycad/models/unit_illuminance_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_length_format.py` & `kittycad-0.4.1/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_mass_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_mass_format.py` & `kittycad-0.4.1/kittycad/models/unit_mass_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_metric_power.py` & `kittycad-0.4.1/kittycad/models/unit_metric_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_metric_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_power_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_pressure_format.py` & `kittycad-0.4.1/kittycad/models/unit_pressure_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_radiation_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_radiation_format.py` & `kittycad-0.4.1/kittycad/models/unit_radiation_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_radioactivity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_radioactivity_format.py` & `kittycad-0.4.1/kittycad/models/unit_radioactivity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_solid_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_temperature_format.py` & `kittycad-0.4.1/kittycad/models/unit_temperature_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_time_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_time_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_time_format.py` & `kittycad-0.4.1/kittycad/models/unit_time_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_velocity_format.py` & `kittycad-0.4.1/kittycad/models/unit_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_voltage_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_volume_conversion.py` & `kittycad-0.4.1/kittycad/models/unit_volume_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/unit_volume_format.py` & `kittycad-0.4.1/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/update_user.py` & `kittycad-0.4.1/kittycad/models/update_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/user.py` & `kittycad-0.4.1/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/user_results_page.py` & `kittycad-0.4.1/kittycad/models/user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/models/verification_token.py` & `kittycad-0.4.1/kittycad/models/verification_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/kittycad/types.py` & `kittycad-0.4.1/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.0/pyproject.toml` & `kittycad-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.4.0"
+version = "0.4.1"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
```

### Comparing `kittycad-0.4.0/PKG-INFO` & `kittycad-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.4.0
+Version: 0.4.1
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


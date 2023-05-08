# Comparing `tmp/kittycad-0.3.9.tar.gz` & `tmp/kittycad-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.3.9.tar", max compression
+gzip compressed data, was "kittycad-0.4.0.tar", max compression
```

## Comparing `kittycad-0.3.9.tar` & `kittycad-0.4.0.tar`

### file list

```diff
@@ -1,271 +1,271 @@
--rw-r--r--   0        0        0     1065 2023-05-04 08:24:50.530608 kittycad-0.3.9/LICENSE
--rw-r--r--   0        0        0      875 2023-05-04 08:24:50.530608 kittycad-0.3.9/README.md
--rw-r--r--   0        0        0       48 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3747 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3525 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2771 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3215 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6031 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4208 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4977 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4787 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4323 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2551 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2976 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2762 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4256 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2883 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2435 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      142 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/__init__.py
--rw-r--r--   0        0        0     2752 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/cmd.py
--rw-r--r--   0        0        0     2656 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/cmd_batch.py
--rw-r--r--   0        0        0      161 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1930 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3173 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4433 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     4254 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     4272 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3827 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3763 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3317 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2236 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2607 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2530 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2159 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2211 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      123 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2610 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2528 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2583 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2627 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2659 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2588 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2656 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2932 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2580 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3938 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     4023 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3730 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     4054 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3806 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3754 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3910 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     4202 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3943 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3890 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3927 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3820 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3754 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3832 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3858 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3891 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3910 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3832 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3806 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2676 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2735 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3027 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3157 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2446 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2484 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2489 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2601 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4077 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4159 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2745 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/client.py
--rw-r--r--   0        0        0     4725 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/client_test.py
--rw-r--r--   0        0        0    86464 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/examples_test.py
--rw-r--r--   0        0        0     7838 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8266 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3278 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5747 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34040 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/customer.py
--rw-r--r--   0        0        0     4306 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     3553 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd.py
--rw-r--r--   0        0        0       75 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_id.py
--rw-r--r--   0        0        0     2441 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_req.py
--rw-r--r--   0        0        0     1746 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_req_batch.py
--rw-r--r--   0        0        0     2393 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_error.py
--rw-r--r--   0        0        0     1869 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_outcome.py
--rw-r--r--   0        0        0     1505 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_outcomes.py
--rw-r--r--   0        0        0     1789 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      269 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     5700 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6060 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5725 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5707 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5522 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5428 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1337 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/method.py
--rw-r--r--   0        0        0     3081 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2501 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5424 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1498 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3638 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6317 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      642 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      916 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6360 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      754 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      888 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      380 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6330 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      752 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      539 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6377 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      656 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6252 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0     1488 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0     1162 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      645 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6304 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      584 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     2187 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6442 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      402 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6321 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      389 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1094 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0     3438 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6259 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6287 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6297 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      468 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6265 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      725 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6278 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      586 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6330 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      570 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6295 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      500 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6304 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      674 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      902 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6265 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      753 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6252 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      452 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     3286 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2577 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/types.py
--rw-r--r--   0        0        0     2416 2023-05-04 08:24:50.958633 kittycad-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-08 20:06:09.479519 kittycad-0.4.0/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-08 20:06:09.479519 kittycad-0.4.0/README.md
+-rw-r--r--   0        0        0       48 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3781 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3559 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3110 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2799 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3243 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6149 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4236 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5005 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4815 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4351 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-08 20:06:09.899528 kittycad-0.4.0/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2879 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2784 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4284 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2911 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2338 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      142 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/__init__.py
+-rw-r--r--   0        0        0     2786 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/cmd.py
+-rw-r--r--   0        0        0     2684 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/drawing/cmd_batch.py
+-rw-r--r--   0        0        0      161 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1781 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3195 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     3871 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4461 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     4276 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     4294 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3855 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3785 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3220 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2139 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2383 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2629 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2564 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2193 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2245 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      123 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2956 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2638 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2431 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2655 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2681 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2616 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2684 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2954 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2483 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3966 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3784 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     4051 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3758 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     4082 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     4230 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3971 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3918 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3955 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3848 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3886 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3919 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2757 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3061 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3185 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2480 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2506 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2523 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2629 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4105 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4187 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2779 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/client.py
+-rw-r--r--   0        0        0     5250 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/client_test.py
+-rw-r--r--   0        0        0   127516 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/examples_test.py
+-rw-r--r--   0        0        0     7838 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-08 20:06:09.903528 kittycad-0.4.0/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8266 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3278 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5747 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34040 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4306 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     3553 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd.py
+-rw-r--r--   0        0        0       75 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_id.py
+-rw-r--r--   0        0        0     2441 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_req.py
+-rw-r--r--   0        0        0     1746 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_cmd_req_batch.py
+-rw-r--r--   0        0        0     2393 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_error.py
+-rw-r--r--   0        0        0     1869 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_outcome.py
+-rw-r--r--   0        0        0     1505 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/drawing_outcomes.py
+-rw-r--r--   0        0        0     1789 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      269 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     5700 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6060 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5725 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5707 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5522 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5428 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1337 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/method.py
+-rw-r--r--   0        0        0     3081 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2501 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5424 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1498 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3638 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-08 20:06:09.907528 kittycad-0.4.0/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6317 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      642 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6360 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      754 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      888 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      380 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6330 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      752 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      539 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6377 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      656 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6252 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0     1488 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0     1162 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      645 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6304 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      584 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     2187 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6442 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      402 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6321 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      389 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1094 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0     3438 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6259 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6287 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6297 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6226 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      468 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6265 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      725 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6278 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      586 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6330 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      570 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6295 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      500 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6304 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      674 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6213 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      902 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6265 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      753 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6252 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      452 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6239 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     3286 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2577 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-08 20:06:09.911528 kittycad-0.4.0/kittycad/types.py
+-rw-r--r--   0        0        0     2472 2023-05-08 20:06:09.911528 kittycad-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.0/PKG-INFO
```

### Comparing `kittycad-0.3.9/LICENSE` & `kittycad-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/README.md` & `kittycad-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.0/kittycad/api/ai/create_image_to_3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,43 +29,45 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Mesh, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Mesh, Error]]:
     if response.status_code == 200:
         response_200 = Mesh.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Mesh, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[Mesh, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     input_format: ImageType,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Optional[Union[Mesh, Error]]]:
     kwargs = _get_kwargs(
         input_format=input_format,
         output_format=output_format,
         body=body,
         client=client,
     )
 
@@ -79,15 +81,15 @@
 
 def sync(
     input_format: ImageType,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Mesh, Error]]:
     """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
     return sync_detailed(
         input_format=input_format,
         output_format=output_format,
         body=body,
         client=client,
@@ -96,15 +98,15 @@
 
 async def asyncio_detailed(
     input_format: ImageType,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Optional[Union[Mesh, Error]]]:
     kwargs = _get_kwargs(
         input_format=input_format,
         output_format=output_format,
         body=body,
         client=client,
     )
 
@@ -116,15 +118,15 @@
 
 async def asyncio(
     input_format: ImageType,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Mesh, Error]]:
     """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             input_format=input_format,
             output_format=output_format,
             body=body,
```

### Comparing `kittycad-0.3.9/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.0/kittycad/api/ai/create_text_to_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,42 +31,44 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Mesh, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Mesh, Error]]:
     if response.status_code == 200:
         response_200 = Mesh.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Mesh, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[Mesh, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: FileExportFormat,
     prompt: str,
     *,
     client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Optional[Union[Mesh, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         prompt=prompt,
         client=client,
     )
 
     response = httpx.post(
@@ -78,30 +80,30 @@
 
 
 def sync(
     output_format: FileExportFormat,
     prompt: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Mesh, Error]]:
     """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         prompt=prompt,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     output_format: FileExportFormat,
     prompt: str,
     *,
     client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Optional[Union[Mesh, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         prompt=prompt,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -111,15 +113,15 @@
 
 
 async def asyncio(
     output_format: FileExportFormat,
     prompt: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Mesh, Error]]:
     """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             prompt=prompt,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.0/kittycad/api/api_calls/get_api_call.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,43 +24,43 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     if response.status_code == 200:
         response_200 = ApiCallWithPrice.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
@@ -70,30 +70,30 @@
     return _build_response(response=response)
 
 
 def sync(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user.
     If the user is not authenticated to view the specified API call, then it is not returned.
     Only KittyCAD employees can view API calls for other users."""  # noqa: E501
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
@@ -101,15 +101,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user.
     If the user is not authenticated to view the specified API call, then it is not returned.
     Only KittyCAD employees can view API calls for other users."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             id=id,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.0/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,43 +24,43 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     if response.status_code == 200:
         response_200 = ApiCallWithPrice.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
@@ -70,28 +70,28 @@
     return _build_response(response=response)
 
 
 def sync(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user."""  # noqa: E501
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
+) -> Response[Optional[Union[ApiCallWithPrice, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
@@ -99,15 +99,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
+) -> Optional[Union[ApiCallWithPrice, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.0/kittycad/api/apps/apps_github_consent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,107 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.api_call_query_group import ApiCallQueryGroup
-from ...models.api_call_query_group_by import ApiCallQueryGroupBy
+from ...models.app_client_info import AppClientInfo
 from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
-    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api-call-metrics".format(client.base_url)  # noqa: E501
-    if group_by is not None:
-        if "?" in url:
-            url = url + "&group_by=" + str(group_by)
-        else:
-            url = url + "?group_by=" + str(group_by)
+    url = "{}/apps/github/consent".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, List[ApiCallQueryGroup], Error]]:
+) -> Optional[Union[AppClientInfo, Error]]:
     if response.status_code == 200:
-        response_200 = [ApiCallQueryGroup.from_dict(item) for item in response.json()]
+        response_200 = AppClientInfo.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, List[ApiCallQueryGroup], Error]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Response[Union[Any, List[ApiCallQueryGroup], Error]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     kwargs = _get_kwargs(
-        group_by=group_by,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Optional[Union[Any, List[ApiCallQueryGroup], Error]]:
-    """This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed."""  # noqa: E501
+) -> Optional[Union[AppClientInfo, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
 
     return sync_detailed(
-        group_by=group_by,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Response[Union[Any, List[ApiCallQueryGroup], Error]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     kwargs = _get_kwargs(
-        group_by=group_by,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Optional[Union[Any, List[ApiCallQueryGroup], Error]]:
-    """This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed."""  # noqa: E501
+) -> Optional[Union[AppClientInfo, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            group_by=group_by,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.0/kittycad/api/api_calls/get_async_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     }
 
 
 def _parse_response(
     *, response: httpx.Response
 ) -> Optional[
     Union[
-        Any,
         FileConversion,
         FileCenterOfMass,
         FileMass,
         FileVolume,
         FileDensity,
         FileSurfaceArea,
         Error,
@@ -103,29 +102,30 @@
             raise
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
 ) -> Response[
-    Union[
-        Any,
-        FileConversion,
-        FileCenterOfMass,
-        FileMass,
-        FileVolume,
-        FileDensity,
-        FileSurfaceArea,
-        Error,
+    Optional[
+        Union[
+            FileConversion,
+            FileCenterOfMass,
+            FileMass,
+            FileVolume,
+            FileDensity,
+            FileSurfaceArea,
+            Error,
+        ]
     ]
 ]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
@@ -133,23 +133,24 @@
 
 
 def sync_detailed(
     id: str,
     *,
     client: Client,
 ) -> Response[
-    Union[
-        Any,
-        FileConversion,
-        FileCenterOfMass,
-        FileMass,
-        FileVolume,
-        FileDensity,
-        FileSurfaceArea,
-        Error,
+    Optional[
+        Union[
+            FileConversion,
+            FileCenterOfMass,
+            FileMass,
+            FileVolume,
+            FileDensity,
+            FileSurfaceArea,
+            Error,
+        ]
     ]
 ]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
@@ -163,15 +164,14 @@
 
 def sync(
     id: str,
     *,
     client: Client,
 ) -> Optional[
     Union[
-        Any,
         FileConversion,
         FileCenterOfMass,
         FileMass,
         FileVolume,
         FileDensity,
         FileSurfaceArea,
         Error,
@@ -189,23 +189,24 @@
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: Client,
 ) -> Response[
-    Union[
-        Any,
-        FileConversion,
-        FileCenterOfMass,
-        FileMass,
-        FileVolume,
-        FileDensity,
-        FileSurfaceArea,
-        Error,
+    Optional[
+        Union[
+            FileConversion,
+            FileCenterOfMass,
+            FileMass,
+            FileVolume,
+            FileDensity,
+            FileSurfaceArea,
+            Error,
+        ]
     ]
 ]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
@@ -217,15 +218,14 @@
 
 async def asyncio(
     id: str,
     *,
     client: Client,
 ) -> Optional[
     Union[
-        Any,
         FileConversion,
         FileCenterOfMass,
         FileMass,
         FileVolume,
         FileDensity,
         FileSurfaceArea,
         Error,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.0/kittycad/api/api_calls/list_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,45 +42,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = ApiCallWithPriceResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -94,15 +94,15 @@
 
 def sync(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by a KittyCAD employee. The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
@@ -111,15 +111,15 @@
 
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -131,15 +131,15 @@
 
 async def asyncio(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by a KittyCAD employee. The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.0/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,30 +43,30 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = ApiCallWithPriceResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
@@ -74,15 +74,15 @@
 def sync_detailed(
     id: str,
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
@@ -98,15 +98,15 @@
 def sync(
     id: str,
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user if "me" is passed as the user id.
     Alternatively, you can use the `/user/api-calls` endpoint to get the API calls for your user.
     If the authenticated user is a KittyCAD employee, then the API calls are returned for the user specified by the user id.
     The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return sync_detailed(
         id=id,
@@ -120,15 +120,15 @@
 async def asyncio_detailed(
     id: str,
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
@@ -142,15 +142,15 @@
 async def asyncio(
     id: str,
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user if "me" is passed as the user id.
     Alternatively, you can use the `/user/api-calls` endpoint to get the API calls for your user.
     If the authenticated user is a KittyCAD employee, then the API calls are returned for the user specified by the user id.
     The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.0/kittycad/api/api_calls/list_async_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,30 +49,30 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Optional[Union[AsyncApiCallResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = AsyncApiCallResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Response[Optional[Union[AsyncApiCallResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
@@ -80,15 +80,15 @@
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     status: ApiCallStatus,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Response[Optional[Union[AsyncApiCallResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         status=status,
         client=client,
     )
@@ -104,15 +104,15 @@
 def sync(
     sort_by: CreatedAtSortMode,
     status: ApiCallStatus,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Optional[Union[AsyncApiCallResultsPage, Error]]:
     """For async file conversion operations, this endpoint does not return the contents of converted files (`output`). To get the contents use the `/async/operations/{id}` endpoint.
     This endpoint requires authentication by a KittyCAD employee."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
@@ -124,15 +124,15 @@
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     status: ApiCallStatus,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Response[Optional[Union[AsyncApiCallResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         status=status,
         client=client,
     )
@@ -146,15 +146,15 @@
 async def asyncio(
     sort_by: CreatedAtSortMode,
     status: ApiCallStatus,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
+) -> Optional[Union[AsyncApiCallResultsPage, Error]]:
     """For async file conversion operations, this endpoint does not return the contents of converted files (`output`). To get the contents use the `/async/operations/{id}` endpoint.
     This endpoint requires authentication by a KittyCAD employee."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.0/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,45 +42,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = ApiCallWithPriceResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -94,15 +94,15 @@
 
 def sync(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user.
     The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
@@ -112,15 +112,15 @@
 
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Response[Optional[Union[ApiCallWithPriceResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -132,15 +132,15 @@
 
 async def asyncio(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiCallWithPriceResultsPage, Error]]:
+) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user.
     The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.0/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,44 +21,42 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, ApiToken, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[ApiToken, Error]]:
     if response.status_code == 201:
         response_201 = ApiToken.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,40 +64,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
+) -> Optional[Union[ApiToken, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It creates a new API token for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
+) -> Optional[Union[ApiToken, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It creates a new API token for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.0/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -23,41 +23,39 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     response = httpx.delete(
         verify=client.verify_ssl,
@@ -67,29 +65,29 @@
     return _build_response(response=response)
 
 
 def sync(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
     This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
 
     return sync_detailed(
         token=token,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.delete(**kwargs)
@@ -97,15 +95,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
     This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             token=token,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.0/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,45 +24,43 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, ApiToken, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[ApiToken, Error]]:
     if response.status_code == 200:
         response_200 = ApiToken.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
@@ -72,28 +70,28 @@
     return _build_response(response=response)
 
 
 def sync(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
+) -> Optional[Union[ApiToken, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return sync_detailed(
         token=token,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
+) -> Response[Optional[Union[ApiToken, Error]]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
@@ -101,15 +99,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
+) -> Optional[Union[ApiToken, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             token=token,
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.0/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,45 +42,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Optional[Union[ApiTokenResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = ApiTokenResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Response[Optional[Union[ApiTokenResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Response[Optional[Union[ApiTokenResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -94,15 +94,15 @@
 
 def sync(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Optional[Union[ApiTokenResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API tokens for the authenticated user.
     The API tokens are returned in order of creation, with the most recently created API tokens first."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
@@ -112,15 +112,15 @@
 
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Response[Optional[Union[ApiTokenResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -132,15 +132,15 @@
 
 async def asyncio(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ApiTokenResultsPage, Error]]:
+) -> Optional[Union[ApiTokenResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API tokens for the authenticated user.
     The API tokens are returned in order of creation, with the most recently created API tokens first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
```

### Comparing `kittycad-0.3.9/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.0/kittycad/api/apps/apps_github_callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -20,40 +20,38 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,41 +59,41 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
     The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
     The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.0/kittycad/api/constant/get_physics_constant.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,115 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.app_client_info import AppClientInfo
 from ...models.error import Error
+from ...models.physics_constant import PhysicsConstant
+from ...models.physics_constant_name import PhysicsConstantName
 from ...types import Response
 
 
 def _get_kwargs(
+    constant: PhysicsConstantName,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/apps/github/consent".format(client.base_url)  # noqa: E501
+    url = "{}/constant/physics/{constant}".format(
+        client.base_url, constant=constant
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, AppClientInfo, Error]]:
+) -> Optional[Union[PhysicsConstant, Error]]:
     if response.status_code == 200:
-        response_200 = AppClientInfo.from_dict(response.json())
+        response_200 = PhysicsConstant.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, AppClientInfo, Error]]:
+) -> Response[Optional[Union[PhysicsConstant, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    constant: PhysicsConstantName,
     *,
     client: Client,
-) -> Response[Union[Any, AppClientInfo, Error]]:
+) -> Response[Optional[Union[PhysicsConstant, Error]]]:
     kwargs = _get_kwargs(
+        constant=constant,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    constant: PhysicsConstantName,
     *,
     client: Client,
-) -> Optional[Union[Any, AppClientInfo, Error]]:
-    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+) -> Optional[Union[PhysicsConstant, Error]]:
 
     return sync_detailed(
+        constant=constant,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    constant: PhysicsConstantName,
     *,
     client: Client,
-) -> Response[Union[Any, AppClientInfo, Error]]:
+) -> Response[Optional[Union[PhysicsConstant, Error]]]:
     kwargs = _get_kwargs(
+        constant=constant,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    constant: PhysicsConstantName,
     *,
     client: Client,
-) -> Optional[Union[Any, AppClientInfo, Error]]:
-    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+) -> Optional[Union[PhysicsConstant, Error]]:
 
     return (
         await asyncio_detailed(
+            constant=constant,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.0/kittycad/api/apps/apps_github_webhook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -22,41 +22,39 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
@@ -66,28 +64,28 @@
     return _build_response(response=response)
 
 
 def sync(
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """These come from the GitHub app."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
@@ -95,15 +93,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """These come from the GitHub app."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.0/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,107 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.physics_constant import PhysicsConstant
-from ...models.physics_constant_name import PhysicsConstantName
 from ...types import Response
 
 
 def _get_kwargs(
-    constant: PhysicsConstantName,
+    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/constant/physics/{constant}".format(
-        client.base_url, constant=constant
-    )  # noqa: E501
+    url = "{}/user/payment/methods/{id}".format(client.base_url, id=id)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, PhysicsConstant, Error]]:
-    if response.status_code == 200:
-        response_200 = PhysicsConstant.from_dict(response.json())
-        return response_200
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, PhysicsConstant, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    constant: PhysicsConstantName,
+    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, PhysicsConstant, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
-        constant=constant,
+        id=id,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.delete(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    constant: PhysicsConstantName,
+    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, PhysicsConstant, Error]]:
+) -> Optional[Error]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
-        constant=constant,
+        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    constant: PhysicsConstantName,
+    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, PhysicsConstant, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
-        constant=constant,
+        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.delete(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    constant: PhysicsConstantName,
+    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, PhysicsConstant, Error]]:
+) -> Optional[Error]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            constant=constant,
+            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/drawing/cmd.py` & `kittycad-0.4.0/kittycad/api/drawing/cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,41 +23,43 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
     if response.status_code == 200:
         response_200 = response.json()
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[dict, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     body: DrawingCmdReq,
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
@@ -67,28 +69,28 @@
     return _build_response(response=response)
 
 
 def sync(
     body: DrawingCmdReq,
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
     """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     body: DrawingCmdReq,
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
@@ -96,15 +98,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     body: DrawingCmdReq,
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
     """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/drawing/cmd_batch.py` & `kittycad-0.4.0/kittycad/api/drawing/cmd_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,43 +26,43 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, DrawingOutcomes, Error]]:
+) -> Optional[Union[DrawingOutcomes, Error]]:
     if response.status_code == 200:
         response_200 = DrawingOutcomes.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, DrawingOutcomes, Error]]:
+) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     body: DrawingCmdReqBatch,
     *,
     client: Client,
-) -> Response[Union[Any, DrawingOutcomes, Error]]:
+) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
@@ -72,27 +72,27 @@
     return _build_response(response=response)
 
 
 def sync(
     body: DrawingCmdReqBatch,
     *,
     client: Client,
-) -> Optional[Union[Any, DrawingOutcomes, Error]]:
+) -> Optional[Union[DrawingOutcomes, Error]]:
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     body: DrawingCmdReqBatch,
     *,
     client: Client,
-) -> Response[Union[Any, DrawingOutcomes, Error]]:
+) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
@@ -100,15 +100,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     body: DrawingCmdReqBatch,
     *,
     client: Client,
-) -> Optional[Union[Any, DrawingOutcomes, Error]]:
+) -> Optional[Union[DrawingOutcomes, Error]]:
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.0/kittycad/api/executor/create_executor_term.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict
 
 import httpx
 
 from ...client import Client
 from ...types import Response
 
 
@@ -19,36 +19,31 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any,]]:
-    return None
-    return None
+def _parse_response(*, response: httpx.Response):
+    return
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any,]]:
+def _build_response(*, response: httpx.Response) -> Response[Any]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any,]]:
+) -> Response[Any]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -56,40 +51,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any,]]:
+):
     """Attach to a docker container to create an interactive terminal."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any,]]:
+) -> Response[Any]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any,]]:
+):
     """Attach to a docker container to create an interactive terminal."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.0/kittycad/api/executor/create_file_execution.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,47 +31,45 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, CodeOutput, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[CodeOutput, Error]]:
     if response.status_code == 200:
         response_200 = CodeOutput.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, CodeOutput, Error]]:
+) -> Response[Optional[Union[CodeOutput, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
-) -> Response[Union[Any, CodeOutput, Error]]:
+) -> Response[Optional[Union[CodeOutput, Error]]]:
     kwargs = _get_kwargs(
         lang=lang,
         output=output,
         body=body,
         client=client,
     )
 
@@ -85,15 +83,15 @@
 
 def sync(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
-) -> Optional[Union[Any, CodeOutput, Error]]:
+) -> Optional[Union[CodeOutput, Error]]:
 
     return sync_detailed(
         lang=lang,
         output=output,
         body=body,
         client=client,
     ).parsed
@@ -101,15 +99,15 @@
 
 async def asyncio_detailed(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
-) -> Response[Union[Any, CodeOutput, Error]]:
+) -> Response[Optional[Union[CodeOutput, Error]]]:
     kwargs = _get_kwargs(
         lang=lang,
         output=output,
         body=body,
         client=client,
     )
 
@@ -121,15 +119,15 @@
 
 async def asyncio(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
-) -> Optional[Union[Any, CodeOutput, Error]]:
+) -> Optional[Union[CodeOutput, Error]]:
 
     return (
         await asyncio_detailed(
             lang=lang,
             output=output,
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.0/kittycad/api/file/create_file_surface_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.file_center_of_mass import FileCenterOfMass
 from ...models.file_import_format import FileImportFormat
+from ...models.file_surface_area import FileSurfaceArea
 from ...types import Response
 
 
 def _get_kwargs(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/center-of-mass".format(client.base_url)  # noqa: E501
+    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -32,44 +32,44 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, FileCenterOfMass, Error]]:
+) -> Optional[Union[FileSurfaceArea, Error]]:
     if response.status_code == 201:
-        response_201 = FileCenterOfMass.from_dict(response.json())
+        response_201 = FileSurfaceArea.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileCenterOfMass, Error]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileCenterOfMass, Error]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
@@ -81,31 +81,31 @@
 
 
 def sync(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileCenterOfMass, Error]]:
-    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileSurfaceArea, Error]]:
+    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileCenterOfMass, Error]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -115,16 +115,16 @@
 
 
 async def asyncio(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileCenterOfMass, Error]]:
-    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileSurfaceArea, Error]]:
+    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.0/kittycad/api/file/create_file_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,45 +31,45 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, FileConversion, Error]]:
+) -> Optional[Union[FileConversion, Error]]:
     if response.status_code == 201:
         response_201 = FileConversion.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileConversion, Error]]:
+) -> Response[Optional[Union[FileConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileConversion, Error]]:
+) -> Response[Optional[Union[FileConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -83,15 +83,15 @@
 
 def sync(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileConversion, Error]]:
+) -> Optional[Union[FileConversion, Error]]:
     """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
@@ -102,15 +102,15 @@
 
 async def asyncio_detailed(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileConversion, Error]]:
+) -> Response[Optional[Union[FileConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -122,15 +122,15 @@
 
 async def asyncio(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileConversion, Error]]:
+) -> Optional[Union[FileConversion, Error]]:
     """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.0/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_density.py` & `kittycad-0.4.0/kittycad/api/file/create_file_density.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,47 +36,45 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, FileDensity, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[FileDensity, Error]]:
     if response.status_code == 201:
         response_201 = FileDensity.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileDensity, Error]]:
+) -> Response[Optional[Union[FileDensity, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileDensity, Error]]:
+) -> Response[Optional[Union[FileDensity, Error]]]:
     kwargs = _get_kwargs(
         material_mass=material_mass,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -90,15 +88,15 @@
 
 def sync(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileDensity, Error]]:
+) -> Optional[Union[FileDensity, Error]]:
     """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         material_mass=material_mass,
         src_format=src_format,
         body=body,
@@ -108,15 +106,15 @@
 
 async def asyncio_detailed(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileDensity, Error]]:
+) -> Response[Optional[Union[FileDensity, Error]]]:
     kwargs = _get_kwargs(
         material_mass=material_mass,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -128,15 +126,15 @@
 
 async def asyncio(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileDensity, Error]]:
+) -> Optional[Union[FileDensity, Error]]:
     """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             material_mass=material_mass,
             src_format=src_format,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_mass.py` & `kittycad-0.4.0/kittycad/api/file/create_file_mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,47 +36,45 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, FileMass, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[FileMass, Error]]:
     if response.status_code == 201:
         response_201 = FileMass.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileMass, Error]]:
+) -> Response[Optional[Union[FileMass, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
+) -> Response[Optional[Union[FileMass, Error]]]:
     kwargs = _get_kwargs(
         material_density=material_density,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -90,15 +88,15 @@
 
 def sync(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
+) -> Optional[Union[FileMass, Error]]:
     """Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         material_density=material_density,
         src_format=src_format,
         body=body,
@@ -108,15 +106,15 @@
 
 async def asyncio_detailed(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
+) -> Response[Optional[Union[FileMass, Error]]]:
     kwargs = _get_kwargs(
         material_density=material_density,
         src_format=src_format,
         body=body,
         client=client,
     )
 
@@ -128,15 +126,15 @@
 
 async def asyncio(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
+) -> Optional[Union[FileMass, Error]]:
     """Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             material_density=material_density,
             src_format=src_format,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.0/kittycad/api/file/create_file_volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.file_import_format import FileImportFormat
-from ...models.file_surface_area import FileSurfaceArea
+from ...models.file_volume import FileVolume
 from ...types import Response
 
 
 def _get_kwargs(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
+    url = "{}/file/volume".format(client.base_url)  # noqa: E501
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -30,46 +30,44 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, FileSurfaceArea, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[FileVolume, Error]]:
     if response.status_code == 201:
-        response_201 = FileSurfaceArea.from_dict(response.json())
+        response_201 = FileVolume.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileSurfaceArea, Error]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileSurfaceArea, Error]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
@@ -81,31 +79,31 @@
 
 
 def sync(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileSurfaceArea, Error]]:
-    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileVolume, Error]]:
+    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileSurfaceArea, Error]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -115,16 +113,16 @@
 
 
 async def asyncio(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileSurfaceArea, Error]]:
-    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileVolume, Error]]:
+    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/create_file_volume.py` & `kittycad-0.4.0/kittycad/api/file/create_file_center_of_mass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.file_center_of_mass import FileCenterOfMass
 from ...models.file_import_format import FileImportFormat
-from ...models.file_volume import FileVolume
 from ...types import Response
 
 
 def _get_kwargs(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/volume".format(client.base_url)  # noqa: E501
+    url = "{}/file/center-of-mass".format(client.base_url)  # noqa: E501
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -32,44 +32,44 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, FileVolume, Error]]:
+) -> Optional[Union[FileCenterOfMass, Error]]:
     if response.status_code == 201:
-        response_201 = FileVolume.from_dict(response.json())
+        response_201 = FileCenterOfMass.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, FileVolume, Error]]:
+) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileVolume, Error]]:
+) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
@@ -81,31 +81,31 @@
 
 
 def sync(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileVolume, Error]]:
-    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileCenterOfMass, Error]]:
+    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Union[Any, FileVolume, Error]]:
+) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -115,16 +115,16 @@
 
 
 async def asyncio(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[Any, FileVolume, Error]]:
-    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileCenterOfMass, Error]]:
+    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.0/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.0/kittycad/api/meta/ping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,101 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.email_authentication_form import EmailAuthenticationForm
 from ...models.error import Error
-from ...models.verification_token import VerificationToken
+from ...models.pong import Pong
 from ...types import Response
 
 
 def _get_kwargs(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/auth/email".format(client.base_url)  # noqa: E501
+    url = "{}/ping".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, VerificationToken, Error]]:
-    if response.status_code == 201:
-        response_201 = VerificationToken.from_dict(response.json())
-        return response_201
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Pong, Error]]:
+    if response.status_code == 200:
+        response_200 = Pong.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, VerificationToken, Error]]:
+) -> Response[Optional[Union[Pong, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Union[Any, VerificationToken, Error]]:
+) -> Response[Optional[Union[Pong, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[Any, VerificationToken, Error]]:
+) -> Optional[Union[Pong, Error]]:
 
     return sync_detailed(
-        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Union[Any, VerificationToken, Error]]:
+) -> Response[Optional[Union[Pong, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[Any, VerificationToken, Error]]:
+) -> Optional[Union[Pong, Error]]:
 
     return (
         await asyncio_detailed(
-            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.0/kittycad/api/hidden/auth_email_callback.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -38,43 +38,41 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 302:
-        response_302 = None
-        return response_302
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         callback_url=callback_url,
         email=email,
         token=token,
         client=client,
     )
 
@@ -88,15 +86,15 @@
 
 def sync(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
 
     return sync_detailed(
         callback_url=callback_url,
         email=email,
         token=token,
         client=client,
     ).parsed
@@ -104,15 +102,15 @@
 
 async def asyncio_detailed(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         callback_url=callback_url,
         email=email,
         token=token,
         client=client,
     )
 
@@ -124,15 +122,15 @@
 
 async def asyncio(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
 
     return (
         await asyncio_detailed(
             callback_url=callback_url,
             email=email,
             token=token,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/hidden/logout.py` & `kittycad-0.4.0/kittycad/api/users/get_user_front_hash_self.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,94 +7,96 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/logout".format(client.base_url)  # noqa: E501
+    url = "{}/user/front-hash".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Union[str, Error]]:
+    if response.status_code == 200:
+        response_200 = response.text
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[str, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[str, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This is used in logout scenarios."""  # noqa: E501
+) -> Optional[Union[str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[str, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This is used in logout scenarios."""  # noqa: E501
+) -> Optional[Union[str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.0/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,42 +23,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, AiPluginManifest, Error]]:
+) -> Optional[Union[AiPluginManifest, Error]]:
     if response.status_code == 200:
         response_200 = AiPluginManifest.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, AiPluginManifest, Error]]:
+) -> Response[Optional[Union[AiPluginManifest, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, AiPluginManifest, Error]]:
+) -> Response[Optional[Union[AiPluginManifest, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,38 +66,38 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, AiPluginManifest, Error]]:
+) -> Optional[Union[AiPluginManifest, Error]]:
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, AiPluginManifest, Error]]:
+) -> Response[Optional[Union[AiPluginManifest, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, AiPluginManifest, Error]]:
+) -> Optional[Union[AiPluginManifest, Error]]:
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.0/kittycad/api/meta/get_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,44 +21,42 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Metadata, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Metadata, Error]]:
     if response.status_code == 200:
         response_200 = Metadata.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, Metadata, Error]]:
+) -> Response[Optional[Union[Metadata, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Metadata, Error]]:
+) -> Response[Optional[Union[Metadata, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,41 +64,41 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Metadata, Error]]:
+) -> Optional[Union[Metadata, Error]]:
     """This includes information on any of our other distributed systems it is connected to.
     You must be a KittyCAD employee to perform this request."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Metadata, Error]]:
+) -> Response[Optional[Union[Metadata, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Metadata, Error]]:
+) -> Optional[Union[Metadata, Error]]:
     """This includes information on any of our other distributed systems it is connected to.
     You must be a KittyCAD employee to perform this request."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.0/kittycad/api/meta/get_openai_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,40 +20,42 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
     if response.status_code == 200:
         response_200 = response.json()
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[dict, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,40 +63,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
     """This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
     """This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/meta/get_schema.py` & `kittycad-0.4.0/kittycad/api/meta/get_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,40 +20,42 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
     if response.status_code == 200:
         response_200 = response.json()
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[dict, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,38 +63,38 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, dict, Error]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, dict, Error]]:
+) -> Optional[Union[dict, Error]]:
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/meta/ping.py` & `kittycad-0.4.0/kittycad/api/payments/list_invoices_for_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.pong import Pong
+from ...models.invoice import Invoice
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/ping".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/invoices".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Pong, Error]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[List[Invoice], Error]]:
     if response.status_code == 200:
-        response_200 = Pong.from_dict(response.json())
+        response_200 = [Invoice.from_dict(item) for item in response.json()]
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Pong, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[List[Invoice], Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Pong, Error]]:
+) -> Response[Optional[Union[List[Invoice], Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -62,38 +66,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Pong, Error]]:
+) -> Optional[Union[List[Invoice], Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Pong, Error]]:
+) -> Response[Optional[Union[List[Invoice], Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Pong, Error]]:
+) -> Optional[Union[List[Invoice], Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,45 +24,43 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Customer, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Customer, Error]]:
     if response.status_code == 201:
         response_201 = Customer.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     body: BillingInfo,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
@@ -72,29 +70,29 @@
     return _build_response(response=response)
 
 
 def sync(
     body: BillingInfo,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
+) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     body: BillingInfo,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
@@ -102,15 +100,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     body: BillingInfo,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
+) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,42 +23,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, PaymentIntent, Error]]:
+) -> Optional[Union[PaymentIntent, Error]]:
     if response.status_code == 201:
         response_201 = PaymentIntent.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, PaymentIntent, Error]]:
+) -> Response[Optional[Union[PaymentIntent, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, PaymentIntent, Error]]:
+) -> Response[Optional[Union[PaymentIntent, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,40 +66,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, PaymentIntent, Error]]:
+) -> Optional[Union[PaymentIntent, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, PaymentIntent, Error]]:
+) -> Response[Optional[Union[PaymentIntent, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, PaymentIntent, Error]]:
+) -> Optional[Union[PaymentIntent, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -20,40 +20,38 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.delete(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,41 +59,41 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.delete(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.0/kittycad/api/users/get_user_onboarding_self.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,103 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.onboarding import Onboarding
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/methods/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/user/onboarding".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Onboarding, Error]]:
+    if response.status_code == 200:
+        response_200 = Onboarding.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[Onboarding, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
-    response = httpx.delete(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return sync_detailed(
-        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.delete(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,42 +23,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, CustomerBalance, Error]]:
+) -> Optional[Union[CustomerBalance, Error]]:
     if response.status_code == 200:
         response_200 = CustomerBalance.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, CustomerBalance, Error]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, CustomerBalance, Error]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,40 +66,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, CustomerBalance, Error]]:
+) -> Optional[Union[CustomerBalance, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, CustomerBalance, Error]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, CustomerBalance, Error]]:
+) -> Optional[Union[CustomerBalance, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.0/kittycad/api/hidden/logout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,98 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
-from ...models.customer import Customer
 from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/logout".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Customer, Error]]:
-    if response.status_code == 200:
-        response_200 = Customer.from_dict(response.json())
-        return response_200
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, Customer, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
-    """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+) -> Optional[Error]:
+    """This is used in logout scenarios."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
-    """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+) -> Optional[Error]:
+    """This is used in logout scenarios."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.0/kittycad/api/users/update_user_self.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,114 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.invoice import Invoice
+from ...models.update_user import UpdateUser
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
+    body: UpdateUser,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/invoices".format(client.base_url)  # noqa: E501
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, List[Invoice], Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
     if response.status_code == 200:
-        response_200 = [Invoice.from_dict(item) for item in response.json()]
+        response_200 = User.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, List[Invoice], Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Union[Any, List[Invoice], Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Any, List[Invoice], Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return sync_detailed(
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Union[Any, List[Invoice], Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Any, List[Invoice], Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,42 +23,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, List[PaymentMethod], Error]]:
+) -> Optional[Union[List[PaymentMethod], Error]]:
     if response.status_code == 200:
         response_200 = [PaymentMethod.from_dict(item) for item in response.json()]
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, List[PaymentMethod], Error]]:
+) -> Response[Optional[Union[List[PaymentMethod], Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, List[PaymentMethod], Error]]:
+) -> Response[Optional[Union[List[PaymentMethod], Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,40 +66,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, List[PaymentMethod], Error]]:
+) -> Optional[Union[List[PaymentMethod], Error]]:
     """This endpoint requires authentication by any KittyCAD user. It lists payment methods for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, List[PaymentMethod], Error]]:
+) -> Response[Optional[Union[List[PaymentMethod], Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, List[PaymentMethod], Error]]:
+) -> Optional[Union[List[PaymentMethod], Error]]:
     """This endpoint requires authentication by any KittyCAD user. It lists payment methods for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,45 +24,43 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Customer, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Customer, Error]]:
     if response.status_code == 200:
         response_200 = Customer.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     body: BillingInfo,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.put(
         verify=client.verify_ssl,
@@ -72,29 +70,29 @@
     return _build_response(response=response)
 
 
 def sync(
     body: BillingInfo,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
+) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     body: BillingInfo,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.put(**kwargs)
@@ -102,15 +100,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     body: BillingInfo,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
+) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
     This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.0/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
@@ -20,40 +20,38 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,40 +59,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
+) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Optional[Union[UnitAccelerationConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitAccelerationConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitAccelerationFormat,
     src_format: UnitAccelerationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitAccelerationFormat,
     src_format: UnitAccelerationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Optional[Union[UnitAccelerationConversion, Error]]:
     """Convert an acceleration unit value to another acceleration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitAccelerationFormat,
     src_format: UnitAccelerationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitAccelerationFormat,
     src_format: UnitAccelerationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAccelerationConversion, Error]]:
+) -> Optional[Union[UnitAccelerationConversion, Error]]:
     """Convert an acceleration unit value to another acceleration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_angle_conversion import UnitAngleConversion
-from ...models.unit_angle_format import UnitAngleFormat
+from ...models.unit_energy_conversion import UnitEnergyConversion
+from ...models.unit_energy_format import UnitEnergyFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    output_format: UnitEnergyFormat,
+    src_format: UnitEnergyFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/angle/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/energy/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitAngleConversion, Error]]:
+) -> Optional[Union[UnitEnergyConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitAngleConversion.from_dict(response.json())
+        response_200 = UnitEnergyConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitEnergyConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    output_format: UnitEnergyFormat,
+    src_format: UnitEnergyFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitEnergyConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    output_format: UnitEnergyFormat,
+    src_format: UnitEnergyFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAngleConversion, Error]]:
-    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitEnergyConversion, Error]]:
+    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    output_format: UnitEnergyFormat,
+    src_format: UnitEnergyFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitEnergyConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    output_format: UnitEnergyFormat,
+    src_format: UnitEnergyFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAngleConversion, Error]]:
-    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitEnergyConversion, Error]]:
+    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitAngularVelocityConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitAngularVelocityFormat,
     src_format: UnitAngularVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitAngularVelocityFormat,
     src_format: UnitAngularVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
     """Convert an angular velocity unit value to another angular velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitAngularVelocityFormat,
     src_format: UnitAngularVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitAngularVelocityFormat,
     src_format: UnitAngularVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAngularVelocityConversion, Error]]:
+) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
     """Convert an angular velocity unit value to another angular velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_area_conversion import UnitAreaConversion
-from ...models.unit_area_format import UnitAreaFormat
+from ...models.unit_data_conversion import UnitDataConversion
+from ...models.unit_data_format import UnitDataFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    output_format: UnitDataFormat,
+    src_format: UnitDataFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/area/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/data/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitAreaConversion, Error]]:
+) -> Optional[Union[UnitDataConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitAreaConversion.from_dict(response.json())
+        response_200 = UnitDataConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitAreaConversion, Error]]:
+) -> Response[Optional[Union[UnitDataConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    output_format: UnitDataFormat,
+    src_format: UnitDataFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAreaConversion, Error]]:
+) -> Response[Optional[Union[UnitDataConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    output_format: UnitDataFormat,
+    src_format: UnitDataFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAreaConversion, Error]]:
-    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitDataConversion, Error]]:
+    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    output_format: UnitDataFormat,
+    src_format: UnitDataFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitAreaConversion, Error]]:
+) -> Response[Optional[Union[UnitDataConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    output_format: UnitDataFormat,
+    src_format: UnitDataFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitAreaConversion, Error]]:
-    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitDataConversion, Error]]:
+    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+) -> Optional[Union[UnitChargeConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitChargeConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitChargeConversion, Error]]:
+) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitChargeFormat,
     src_format: UnitChargeFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitChargeConversion, Error]]:
+) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitChargeFormat,
     src_format: UnitChargeFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+) -> Optional[Union[UnitChargeConversion, Error]]:
     """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitChargeFormat,
     src_format: UnitChargeFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitChargeConversion, Error]]:
+) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitChargeFormat,
     src_format: UnitChargeFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+) -> Optional[Union[UnitChargeConversion, Error]]:
     """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Optional[Union[UnitConcentrationConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitConcentrationConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitConcentrationFormat,
     src_format: UnitConcentrationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitConcentrationFormat,
     src_format: UnitConcentrationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Optional[Union[UnitConcentrationConversion, Error]]:
     """Convert a concentration unit value to another concentration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitConcentrationFormat,
     src_format: UnitConcentrationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitConcentrationFormat,
     src_format: UnitConcentrationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitConcentrationConversion, Error]]:
+) -> Optional[Union[UnitConcentrationConversion, Error]]:
     """Convert a concentration unit value to another concentration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Optional[Union[UnitDataTransferRateConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitDataTransferRateConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Response[Optional[Union[UnitDataTransferRateConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitDataTransferRateFormat,
     src_format: UnitDataTransferRateFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Response[Optional[Union[UnitDataTransferRateConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitDataTransferRateFormat,
     src_format: UnitDataTransferRateFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Optional[Union[UnitDataTransferRateConversion, Error]]:
     """Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitDataTransferRateFormat,
     src_format: UnitDataTransferRateFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Response[Optional[Union[UnitDataTransferRateConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitDataTransferRateFormat,
     src_format: UnitDataTransferRateFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
+) -> Optional[Union[UnitDataTransferRateConversion, Error]]:
     """Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_data_conversion import UnitDataConversion
-from ...models.unit_data_format import UnitDataFormat
+from ...models.unit_radioactivity_conversion import UnitRadioactivityConversion
+from ...models.unit_radioactivity_format import UnitRadioactivityFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    output_format: UnitRadioactivityFormat,
+    src_format: UnitRadioactivityFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/data/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/radioactivity/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitDataConversion, Error]]:
+) -> Optional[Union[UnitRadioactivityConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitDataConversion.from_dict(response.json())
+        response_200 = UnitRadioactivityConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitDataConversion, Error]]:
+) -> Response[Optional[Union[UnitRadioactivityConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    output_format: UnitRadioactivityFormat,
+    src_format: UnitRadioactivityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDataConversion, Error]]:
+) -> Response[Optional[Union[UnitRadioactivityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    output_format: UnitRadioactivityFormat,
+    src_format: UnitRadioactivityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDataConversion, Error]]:
-    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitRadioactivityConversion, Error]]:
+    """Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    output_format: UnitRadioactivityFormat,
+    src_format: UnitRadioactivityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDataConversion, Error]]:
+) -> Response[Optional[Union[UnitRadioactivityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    output_format: UnitRadioactivityFormat,
+    src_format: UnitRadioactivityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDataConversion, Error]]:
-    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitRadioactivityConversion, Error]]:
+    """Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_density_conversion import UnitDensityConversion
-from ...models.unit_density_format import UnitDensityFormat
+from ...models.unit_volume_conversion import UnitVolumeConversion
+from ...models.unit_volume_format import UnitVolumeFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    output_format: UnitVolumeFormat,
+    src_format: UnitVolumeFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/density/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/volume/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitDensityConversion, Error]]:
+) -> Optional[Union[UnitVolumeConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitDensityConversion.from_dict(response.json())
+        response_200 = UnitVolumeConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitDensityConversion, Error]]:
+) -> Response[Optional[Union[UnitVolumeConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    output_format: UnitVolumeFormat,
+    src_format: UnitVolumeFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDensityConversion, Error]]:
+) -> Response[Optional[Union[UnitVolumeConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    output_format: UnitVolumeFormat,
+    src_format: UnitVolumeFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDensityConversion, Error]]:
-    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVolumeConversion, Error]]:
+    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    output_format: UnitVolumeFormat,
+    src_format: UnitVolumeFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitDensityConversion, Error]]:
+) -> Response[Optional[Union[UnitVolumeConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    output_format: UnitVolumeFormat,
+    src_format: UnitVolumeFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitDensityConversion, Error]]:
-    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVolumeConversion, Error]]:
+    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_energy_conversion import UnitEnergyConversion
-from ...models.unit_energy_format import UnitEnergyFormat
+from ...models.unit_voltage_conversion import UnitVoltageConversion
+from ...models.unit_voltage_format import UnitVoltageFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitEnergyFormat,
-    src_format: UnitEnergyFormat,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/energy/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/voltage/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
+) -> Optional[Union[UnitVoltageConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitEnergyConversion.from_dict(response.json())
+        response_200 = UnitVoltageConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+) -> Response[Optional[Union[UnitVoltageConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitEnergyFormat,
-    src_format: UnitEnergyFormat,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+) -> Response[Optional[Union[UnitVoltageConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitEnergyFormat,
-    src_format: UnitEnergyFormat,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
-    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVoltageConversion, Error]]:
+    """Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitEnergyFormat,
-    src_format: UnitEnergyFormat,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+) -> Response[Optional[Union[UnitVoltageConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitEnergyFormat,
-    src_format: UnitEnergyFormat,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
-    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVoltageConversion, Error]]:
+    """Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitForceConversion, Error]]:
+) -> Optional[Union[UnitForceConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitForceConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitForceConversion, Error]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitForceFormat,
     src_format: UnitForceFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitForceConversion, Error]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitForceFormat,
     src_format: UnitForceFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitForceConversion, Error]]:
+) -> Optional[Union[UnitForceConversion, Error]]:
     """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitForceFormat,
     src_format: UnitForceFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitForceConversion, Error]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitForceFormat,
     src_format: UnitForceFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitForceConversion, Error]]:
+) -> Optional[Union[UnitForceConversion, Error]]:
     """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Optional[Union[UnitIlluminanceConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitIlluminanceConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitIlluminanceFormat,
     src_format: UnitIlluminanceFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitIlluminanceFormat,
     src_format: UnitIlluminanceFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Optional[Union[UnitIlluminanceConversion, Error]]:
     """Convert a illuminance unit value to another illuminance unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitIlluminanceFormat,
     src_format: UnitIlluminanceFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitIlluminanceFormat,
     src_format: UnitIlluminanceFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitIlluminanceConversion, Error]]:
+) -> Optional[Union[UnitIlluminanceConversion, Error]]:
     """Convert a illuminance unit value to another illuminance unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+) -> Optional[Union[UnitLengthConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitLengthConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitLengthConversion, Error]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitLengthFormat,
     src_format: UnitLengthFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitLengthConversion, Error]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitLengthFormat,
     src_format: UnitLengthFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+) -> Optional[Union[UnitLengthConversion, Error]]:
     """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitLengthFormat,
     src_format: UnitLengthFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitLengthConversion, Error]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitLengthFormat,
     src_format: UnitLengthFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+) -> Optional[Union[UnitLengthConversion, Error]]:
     """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,45 +38,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Optional[Union[UnitMagneticFieldStrengthConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitMagneticFieldStrengthConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFieldStrengthConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitMagneticFieldStrengthFormat,
     src_format: UnitMagneticFieldStrengthFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFieldStrengthConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -90,15 +90,15 @@
 
 def sync(
     output_format: UnitMagneticFieldStrengthFormat,
     src_format: UnitMagneticFieldStrengthFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Optional[Union[UnitMagneticFieldStrengthConversion, Error]]:
     """Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -107,15 +107,15 @@
 
 async def asyncio_detailed(
     output_format: UnitMagneticFieldStrengthFormat,
     src_format: UnitMagneticFieldStrengthFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFieldStrengthConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -127,15 +127,15 @@
 
 async def asyncio(
     output_format: UnitMagneticFieldStrengthFormat,
     src_format: UnitMagneticFieldStrengthFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+) -> Optional[Union[UnitMagneticFieldStrengthConversion, Error]]:
     """Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Optional[Union[UnitMagneticFluxConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitMagneticFluxConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFluxConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitMagneticFluxFormat,
     src_format: UnitMagneticFluxFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFluxConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitMagneticFluxFormat,
     src_format: UnitMagneticFluxFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Optional[Union[UnitMagneticFluxConversion, Error]]:
     """Convert a magnetic flux unit value to another magnetic flux unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitMagneticFluxFormat,
     src_format: UnitMagneticFluxFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Response[Optional[Union[UnitMagneticFluxConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitMagneticFluxFormat,
     src_format: UnitMagneticFluxFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMagneticFluxConversion, Error]]:
+) -> Optional[Union[UnitMagneticFluxConversion, Error]]:
     """Convert a magnetic flux unit value to another magnetic flux unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_mass_conversion import UnitMassConversion
-from ...models.unit_mass_format import UnitMassFormat
+from ...models.unit_solid_angle_conversion import UnitSolidAngleConversion
+from ...models.unit_solid_angle_format import UnitSolidAngleFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitMassFormat,
-    src_format: UnitMassFormat,
+    output_format: UnitSolidAngleFormat,
+    src_format: UnitSolidAngleFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/mass/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/solid-angle/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMassConversion, Error]]:
+) -> Optional[Union[UnitSolidAngleConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitMassConversion.from_dict(response.json())
+        response_200 = UnitSolidAngleConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMassConversion, Error]]:
+) -> Response[Optional[Union[UnitSolidAngleConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitMassFormat,
-    src_format: UnitMassFormat,
+    output_format: UnitSolidAngleFormat,
+    src_format: UnitSolidAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMassConversion, Error]]:
+) -> Response[Optional[Union[UnitSolidAngleConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitMassFormat,
-    src_format: UnitMassFormat,
+    output_format: UnitSolidAngleFormat,
+    src_format: UnitSolidAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMassConversion, Error]]:
-    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitSolidAngleConversion, Error]]:
+    """Convert a solid angle unit value to another solid angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitMassFormat,
-    src_format: UnitMassFormat,
+    output_format: UnitSolidAngleFormat,
+    src_format: UnitSolidAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMassConversion, Error]]:
+) -> Response[Optional[Union[UnitSolidAngleConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitMassFormat,
-    src_format: UnitMassFormat,
+    output_format: UnitSolidAngleFormat,
+    src_format: UnitSolidAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMassConversion, Error]]:
-    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitSolidAngleConversion, Error]]:
+    """Convert a solid angle unit value to another solid angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
     """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
     """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,45 +36,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitMetricPowerSquaredConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -88,15 +88,15 @@
 
 def sync(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
     """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -105,15 +105,15 @@
 
 async def asyncio_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -125,15 +125,15 @@
 
 async def asyncio(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
     """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitMetricPowerConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerConversion, Error]]:
     """Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitMetricPowerConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitMetricPower,
     src_format: UnitMetricPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Optional[Union[UnitMetricPowerConversion, Error]]:
     """Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+) -> Optional[Union[UnitPowerConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitPowerConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitPowerFormat,
     src_format: UnitPowerFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitPowerFormat,
     src_format: UnitPowerFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+) -> Optional[Union[UnitPowerConversion, Error]]:
     """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitPowerFormat,
     src_format: UnitPowerFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitPowerConversion, Error]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitPowerFormat,
     src_format: UnitPowerFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+) -> Optional[Union[UnitPowerConversion, Error]]:
     """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+) -> Optional[Union[UnitPressureConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitPressureConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitPressureFormat,
     src_format: UnitPressureFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitPressureFormat,
     src_format: UnitPressureFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+) -> Optional[Union[UnitPressureConversion, Error]]:
     """Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitPressureFormat,
     src_format: UnitPressureFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitPressureFormat,
     src_format: UnitPressureFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+) -> Optional[Union[UnitPressureConversion, Error]]:
     """Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitRadiationConversion, Error]]:
+) -> Optional[Union[UnitRadiationConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitRadiationConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitRadiationConversion, Error]]:
+) -> Response[Optional[Union[UnitRadiationConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitRadiationFormat,
     src_format: UnitRadiationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitRadiationConversion, Error]]:
+) -> Response[Optional[Union[UnitRadiationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitRadiationFormat,
     src_format: UnitRadiationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitRadiationConversion, Error]]:
+) -> Optional[Union[UnitRadiationConversion, Error]]:
     """Convert a radiation unit value to another radiation unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitRadiationFormat,
     src_format: UnitRadiationFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitRadiationConversion, Error]]:
+) -> Response[Optional[Union[UnitRadiationConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitRadiationFormat,
     src_format: UnitRadiationFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitRadiationConversion, Error]]:
+) -> Optional[Union[UnitRadiationConversion, Error]]:
     """Convert a radiation unit value to another radiation unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_radioactivity_conversion import UnitRadioactivityConversion
-from ...models.unit_radioactivity_format import UnitRadioactivityFormat
+from ...models.unit_mass_conversion import UnitMassConversion
+from ...models.unit_mass_format import UnitMassFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitRadioactivityFormat,
-    src_format: UnitRadioactivityFormat,
+    output_format: UnitMassFormat,
+    src_format: UnitMassFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/radioactivity/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/mass/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
+) -> Optional[Union[UnitMassConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitRadioactivityConversion.from_dict(response.json())
+        response_200 = UnitMassConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitRadioactivityFormat,
-    src_format: UnitRadioactivityFormat,
+    output_format: UnitMassFormat,
+    src_format: UnitMassFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitRadioactivityFormat,
-    src_format: UnitRadioactivityFormat,
+    output_format: UnitMassFormat,
+    src_format: UnitMassFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
-    """Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitMassConversion, Error]]:
+    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitRadioactivityFormat,
-    src_format: UnitRadioactivityFormat,
+    output_format: UnitMassFormat,
+    src_format: UnitMassFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitRadioactivityFormat,
-    src_format: UnitRadioactivityFormat,
+    output_format: UnitMassFormat,
+    src_format: UnitMassFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
-    """Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitMassConversion, Error]]:
+    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_solid_angle_conversion import UnitSolidAngleConversion
-from ...models.unit_solid_angle_format import UnitSolidAngleFormat
+from ...models.unit_angle_conversion import UnitAngleConversion
+from ...models.unit_angle_format import UnitAngleFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitSolidAngleFormat,
-    src_format: UnitSolidAngleFormat,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/solid-angle/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/angle/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitSolidAngleConversion, Error]]:
+) -> Optional[Union[UnitAngleConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitSolidAngleConversion.from_dict(response.json())
+        response_200 = UnitAngleConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitSolidAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitSolidAngleFormat,
-    src_format: UnitSolidAngleFormat,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitSolidAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitSolidAngleFormat,
-    src_format: UnitSolidAngleFormat,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitSolidAngleConversion, Error]]:
-    """Convert a solid angle unit value to another solid angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitSolidAngleFormat,
-    src_format: UnitSolidAngleFormat,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitSolidAngleConversion, Error]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitSolidAngleFormat,
-    src_format: UnitSolidAngleFormat,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitSolidAngleConversion, Error]]:
-    """Convert a solid angle unit value to another solid angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitTemperatureConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitTemperatureFormat,
     src_format: UnitTemperatureFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitTemperatureFormat,
     src_format: UnitTemperatureFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
     """Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitTemperatureFormat,
     src_format: UnitTemperatureFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitTemperatureFormat,
     src_format: UnitTemperatureFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
     """Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_time_conversion import UnitTimeConversion
-from ...models.unit_time_format import UnitTimeFormat
+from ...models.unit_density_conversion import UnitDensityConversion
+from ...models.unit_density_format import UnitDensityFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitTimeFormat,
-    src_format: UnitTimeFormat,
+    output_format: UnitDensityFormat,
+    src_format: UnitDensityFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/time/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/density/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitTimeConversion, Error]]:
+) -> Optional[Union[UnitDensityConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitTimeConversion.from_dict(response.json())
+        response_200 = UnitDensityConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitTimeConversion, Error]]:
+) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitTimeFormat,
-    src_format: UnitTimeFormat,
+    output_format: UnitDensityFormat,
+    src_format: UnitDensityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitTimeConversion, Error]]:
+) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitTimeFormat,
-    src_format: UnitTimeFormat,
+    output_format: UnitDensityFormat,
+    src_format: UnitDensityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitTimeConversion, Error]]:
-    """Convert a time unit value to another time unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitDensityConversion, Error]]:
+    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitTimeFormat,
-    src_format: UnitTimeFormat,
+    output_format: UnitDensityFormat,
+    src_format: UnitDensityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitTimeConversion, Error]]:
+) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitTimeFormat,
-    src_format: UnitTimeFormat,
+    output_format: UnitDensityFormat,
+    src_format: UnitDensityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitTimeConversion, Error]]:
-    """Convert a time unit value to another time unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitDensityConversion, Error]]:
+    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitVelocityConversion, Error]]:
+) -> Optional[Union[UnitVelocityConversion, Error]]:
     if response.status_code == 200:
         response_200 = UnitVelocityConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitVelocityConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     output_format: UnitVelocityFormat,
     src_format: UnitVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitVelocityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -86,15 +86,15 @@
 
 def sync(
     output_format: UnitVelocityFormat,
     src_format: UnitVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitVelocityConversion, Error]]:
+) -> Optional[Union[UnitVelocityConversion, Error]]:
     """Convert a velocity unit value to another velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
@@ -103,15 +103,15 @@
 
 async def asyncio_detailed(
     output_format: UnitVelocityFormat,
     src_format: UnitVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitVelocityConversion, Error]]:
+) -> Response[Optional[Union[UnitVelocityConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -123,15 +123,15 @@
 
 async def asyncio(
     output_format: UnitVelocityFormat,
     src_format: UnitVelocityFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitVelocityConversion, Error]]:
+) -> Optional[Union[UnitVelocityConversion, Error]]:
     """Convert a velocity unit value to another velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
```

### Comparing `kittycad-0.3.9/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.4.0/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_volume_conversion import UnitVolumeConversion
-from ...models.unit_volume_format import UnitVolumeFormat
+from ...models.unit_area_conversion import UnitAreaConversion
+from ...models.unit_area_format import UnitAreaFormat
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitVolumeFormat,
-    src_format: UnitVolumeFormat,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/volume/{src_format}/{output_format}".format(
+    url = "{}/unit/conversion/area/{src_format}/{output_format}".format(
         client.base_url, output_format=output_format, src_format=src_format
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
@@ -34,45 +34,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
+) -> Optional[Union[UnitAreaConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitVolumeConversion.from_dict(response.json())
+        response_200 = UnitAreaConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UnitVolumeConversion, Error]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitVolumeFormat,
-    src_format: UnitVolumeFormat,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitVolumeConversion, Error]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
@@ -81,58 +81,58 @@
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitVolumeFormat,
-    src_format: UnitVolumeFormat,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
-    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAreaConversion, Error]]:
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitVolumeFormat,
-    src_format: UnitVolumeFormat,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
     value: float,
     *,
     client: Client,
-) -> Response[Union[Any, UnitVolumeConversion, Error]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     kwargs = _get_kwargs(
         output_format=output_format,
         src_format=src_format,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitVolumeFormat,
-    src_format: UnitVolumeFormat,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
-    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAreaConversion, Error]]:
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             value=value,
             client=client,
```

### Comparing `kittycad-0.3.9/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.0/kittycad/api/users/get_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,102 +1,116 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/users/{id}".format(client.base_url, id=id)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-    if response.status_code == 204:
-        response_204 = None
-        return response_204
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
+    if response.status_code == 200:
+        response_200 = User.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
-    response = httpx.delete(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
-    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
 
     return sync_detailed(
+        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.delete(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
-    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.0/kittycad/api/users/get_session_for_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,45 +22,43 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Session, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Session, Error]]:
     if response.status_code == 200:
         response_200 = Session.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, Session, Error]]:
+) -> Response[Optional[Union[Session, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Session, Error]]:
+) -> Response[Optional[Union[Session, Error]]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
@@ -70,28 +68,28 @@
     return _build_response(response=response)
 
 
 def sync(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Session, Error]]:
+) -> Optional[Union[Session, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return sync_detailed(
         token=token,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Session, Error]]:
+) -> Response[Optional[Union[Session, Error]]]:
     kwargs = _get_kwargs(
         token=token,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
@@ -99,15 +97,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Session, Error]]:
+) -> Optional[Union[Session, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             token=token,
             client=client,
         )
```

### Comparing `kittycad-0.3.9/kittycad/api/users/get_user.py` & `kittycad-0.4.0/kittycad/api/users/get_user_self.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,110 +5,101 @@
 from ...client import Client
 from ...models.error import Error
 from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/users/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
     if response.status_code == 200:
         response_200 = User.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
-    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
-    Alternatively, to get information about the authenticated user, use `/user` endpoint.
-    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
 
     return sync_detailed(
-        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
-    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
-    Alternatively, to get information about the authenticated user, use `/user` endpoint.
-    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.0/kittycad/api/users/get_user_extended.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,43 +24,43 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ExtendedUser, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     if response.status_code == 200:
         response_200 = ExtendedUser.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ExtendedUser, Error]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ExtendedUser, Error]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
@@ -70,30 +70,30 @@
     return _build_response(response=response)
 
 
 def sync(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ExtendedUser, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
     Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
     To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ExtendedUser, Error]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
@@ -101,15 +101,15 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ExtendedUser, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
     Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
     To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             id=id,
```

### Comparing `kittycad-0.3.9/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.0/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.customer import Customer
 from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/front-hash".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, str, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Customer, Error]]:
     if response.status_code == 200:
-        response_200 = response.text
+        response_200 = Customer.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, str, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[Customer, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, str, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -61,40 +64,42 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, str, Error]]:
-    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
+) -> Optional[Union[Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, str, Error]]:
+) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, str, Error]]:
-    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
+) -> Optional[Union[Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/users/get_user_self.py` & `kittycad-0.4.0/kittycad/api/users/get_user_self_extended.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.user import User
+from ...models.extended_user import ExtendedUser
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/user/extended".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[ExtendedUser, Error]]:
     if response.status_code == 200:
-        response_200 = User.from_dict(response.json())
+        response_200 = ExtendedUser.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -62,42 +66,42 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/api/users/list_users.py` & `kittycad-0.4.0/kittycad/api/users/list_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,45 +42,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, UserResultsPage, Error]]:
+) -> Optional[Union[UserResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = UserResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, UserResultsPage, Error]]:
+) -> Response[Optional[Union[UserResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, UserResultsPage, Error]]:
+) -> Response[Optional[Union[UserResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -94,15 +94,15 @@
 
 def sync(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, UserResultsPage, Error]]:
+) -> Optional[Union[UserResultsPage, Error]]:
     """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
@@ -111,15 +111,15 @@
 
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, UserResultsPage, Error]]:
+) -> Response[Optional[Union[UserResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -131,15 +131,15 @@
 
 async def asyncio(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, UserResultsPage, Error]]:
+) -> Optional[Union[UserResultsPage, Error]]:
     """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
```

### Comparing `kittycad-0.3.9/kittycad/api/users/list_users_extended.py` & `kittycad-0.4.0/kittycad/api/users/list_users_extended.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,45 +42,45 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
     if response.status_code == 200:
         response_200 = ExtendedUserResultsPage.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -94,15 +94,15 @@
 
 def sync(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
     """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
@@ -111,15 +111,15 @@
 
 async def asyncio_detailed(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     kwargs = _get_kwargs(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     )
 
@@ -131,15 +131,15 @@
 
 async def asyncio(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
-) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
     """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
```

### Comparing `kittycad-0.3.9/kittycad/api/users/update_user_self.py` & `kittycad-0.4.0/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,120 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.api_call_query_group import ApiCallQueryGroup
+from ...models.api_call_query_group_by import ApiCallQueryGroupBy
 from ...models.error import Error
-from ...models.update_user import UpdateUser
-from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
-    body: UpdateUser,
+    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/api-call-metrics".format(client.base_url)  # noqa: E501
+    if group_by is not None:
+        if "?" in url:
+            url = url + "&group_by=" + str(group_by)
+        else:
+            url = url + "?group_by=" + str(group_by)
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[List[ApiCallQueryGroup], Error]]:
     if response.status_code == 200:
-        response_200 = User.from_dict(response.json())
+        response_200 = [ApiCallQueryGroup.from_dict(item) for item in response.json()]
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
-    return None
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[List[ApiCallQueryGroup], Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: UpdateUser,
+    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[List[ApiCallQueryGroup], Error]]]:
     kwargs = _get_kwargs(
-        body=body,
+        group_by=group_by,
         client=client,
     )
 
-    response = httpx.put(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: UpdateUser,
+    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Union[List[ApiCallQueryGroup], Error]]:
+    """This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed."""  # noqa: E501
 
     return sync_detailed(
-        body=body,
+        group_by=group_by,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: UpdateUser,
+    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Optional[Union[List[ApiCallQueryGroup], Error]]]:
     kwargs = _get_kwargs(
-        body=body,
+        group_by=group_by,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.put(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: UpdateUser,
+    group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
-) -> Optional[Union[Any, User, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Union[List[ApiCallQueryGroup], Error]]:
+    """This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            body=body,
+            group_by=group_by,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.9/kittycad/client.py` & `kittycad-0.4.0/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/client_test.py` & `kittycad-0.4.0/kittycad/client_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Union
 
 import pytest
 
 from .api.api_tokens import list_api_tokens_for_user
 from .api.file import (
     create_file_conversion_with_base64_helper,
     create_file_mass,
@@ -11,14 +12,15 @@
 from .api.meta import ping
 from .api.users import get_user_self, list_users_extended
 from .client import ClientFromEnv
 from .models import (
     ApiCallStatus,
     ApiTokenResultsPage,
     CreatedAtSortMode,
+    Error,
     ExtendedUserResultsPage,
     FileConversion,
     FileExportFormat,
     FileImportFormat,
     FileMass,
     FileVolume,
     Pong,
@@ -27,92 +29,96 @@
 
 
 def test_get_session():
     # Create our client.
     client = ClientFromEnv()
 
     # Get the session.
-    session: User = get_user_self.sync(client=client)
+    session: Union[User, Error, None] = get_user_self.sync(client=client)
 
-    assert session is not None
+    assert isinstance(session, User)
 
     print(f"Session: {session}")
 
 
 @pytest.mark.asyncio
 async def test_get_api_tokens_async():
     # Create our client.
     client = ClientFromEnv()
 
     # List API tokens.
-    fc: ApiTokenResultsPage = list_api_tokens_for_user.sync(
-        client=client, sort_by=CreatedAtSortMode
+    fc: Union[ApiTokenResultsPage, Error, None] = list_api_tokens_for_user.sync(
+        client=client, sort_by=CreatedAtSortMode.CREATED_AT_ASCENDING
     )
 
-    assert fc is not None
+    assert isinstance(fc, ApiTokenResultsPage)
 
     print(f"fc: {fc}")
 
 
 @pytest.mark.asyncio
 async def test_get_session_async():
     # Create our client.
     client = ClientFromEnv()
 
     # Get the session.
-    session: User = await get_user_self.asyncio(client=client)
+    session: Union[User, Error, None] = await get_user_self.asyncio(client=client)
 
-    assert session is not None
+    assert isinstance(session, User)
 
     print(f"Session: {session}")
 
 
 def test_ping():
     # Create our client.
     client = ClientFromEnv()
 
     # Get the message.
-    message: Pong = ping.sync(client=client)
+    message: Union[Pong, Error, None] = ping.sync(client=client)
 
-    assert message is not None
+    assert isinstance(message, Pong)
 
     print(f"Message: {message}")
 
 
 @pytest.mark.asyncio
 async def test_ping_async():
     # Create our client.
     client = ClientFromEnv()
 
     # Get the message.
-    message: Pong = await ping.asyncio(client=client)
+    message: Union[Pong, Error, None] = await ping.asyncio(client=client)
 
-    assert message is not None
+    assert isinstance(message, Pong)
 
     print(f"Message: {message}")
 
 
 def test_file_convert_stl():
     # Create our client.
     client = ClientFromEnv()
 
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.stl"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
-    fc: FileConversion = create_file_conversion_with_base64_helper.sync(
+    result: Union[
+        FileConversion, Error, None
+    ] = create_file_conversion_with_base64_helper.sync(
         client=client,
         body=content,
         src_format=FileImportFormat.STL,
         output_format=FileExportFormat.OBJ,
     )
 
-    assert fc is not None
+    assert isinstance(result, FileConversion)
+
+    fc: FileConversion = result
 
     print(f"FileConversion: {fc}")
 
     assert fc.id is not None
 
     assert fc.status == ApiCallStatus.COMPLETED
 
@@ -126,22 +132,26 @@
 
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.stl"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
-    fc: FileConversion = await create_file_conversion_with_base64_helper.asyncio(
+    result: Union[
+        FileConversion, Error, None
+    ] = await create_file_conversion_with_base64_helper.asyncio(
         client=client,
         body=content,
         src_format=FileImportFormat.STL,
         output_format=FileExportFormat.OBJ,
     )
 
-    assert fc is not None
+    assert isinstance(result, FileConversion)
+
+    fc: FileConversion = result
 
     print(f"FileConversion: {fc}")
 
     assert fc.id is not None
 
     print(f"FileConversion: {fc}")
 
@@ -152,22 +162,24 @@
 
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.obj"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
-    fm: FileMass = create_file_mass.sync(
+    result: Union[FileMass, Error, None] = create_file_mass.sync(
         client=client,
         body=content,
         src_format=FileImportFormat.OBJ,
         material_density=1.0,
     )
 
-    assert fm is not None
+    assert isinstance(result, FileMass)
+
+    fm: FileMass = result
 
     print(f"FileMass: {fm}")
 
     assert fm.id is not None
     assert fm.mass is not None
 
     assert fm.to_dict() is not None
@@ -181,19 +193,21 @@
 
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.obj"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
-    fv: FileVolume = create_file_volume.sync(
+    result: Union[FileVolume, Error, None] = create_file_volume.sync(
         client=client, body=content, src_format=FileImportFormat.OBJ
     )
 
-    assert fv is not None
+    assert isinstance(result, FileVolume)
+
+    fv: FileVolume = result
 
     print(f"FileVolume: {fv}")
 
     assert fv.id is not None
     assert fv.volume is not None
 
     assert fv.to_dict() is not None
@@ -201,15 +215,14 @@
     assert fv.status == ApiCallStatus.COMPLETED
 
 
 def test_list_users():
     # Create our client.
     client = ClientFromEnv()
 
-    response: ExtendedUserResultsPage = list_users_extended.sync(
+    response: Union[ExtendedUserResultsPage, Error, None] = list_users_extended.sync(
         sort_by=CreatedAtSortMode.CREATED_AT_DESCENDING, client=client, limit=10
     )
 
-    print(f"ExtendedUserResultsPage: {response}")
+    assert isinstance(response, ExtendedUserResultsPage)
 
-    assert response is not None
-    assert response.items is not None
+    print(f"ExtendedUserResultsPage: {response}")
```

### Comparing `kittycad-0.3.9/kittycad/models/__init__.py` & `kittycad-0.4.0/kittycad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.0/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.0/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.0/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_call_query_group.py` & `kittycad-0.4.0/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.0/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_call_status.py` & `kittycad-0.4.0/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_call_with_price.py` & `kittycad-0.4.0/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.0/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_token.py` & `kittycad-0.4.0/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/api_token_results_page.py` & `kittycad-0.4.0/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/app_client_info.py` & `kittycad-0.4.0/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/async_api_call.py` & `kittycad-0.4.0/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/async_api_call_output.py` & `kittycad-0.4.0/kittycad/models/async_api_call_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.0/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/async_api_call_type.py` & `kittycad-0.4.0/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/billing_info.py` & `kittycad-0.4.0/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/cache_metadata.py` & `kittycad-0.4.0/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/card_details.py` & `kittycad-0.4.0/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/cluster.py` & `kittycad-0.4.0/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/code_output.py` & `kittycad-0.4.0/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/commit.py` & `kittycad-0.4.0/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/connection.py` & `kittycad-0.4.0/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/country_code.py` & `kittycad-0.4.0/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/currency.py` & `kittycad-0.4.0/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/customer.py` & `kittycad-0.4.0/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/customer_balance.py` & `kittycad-0.4.0/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.0/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.0/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.0/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/docker_system_info.py` & `kittycad-0.4.0/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_cmd.py` & `kittycad-0.4.0/kittycad/models/drawing_cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_cmd_req.py` & `kittycad-0.4.0/kittycad/models/drawing_cmd_req.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_cmd_req_batch.py` & `kittycad-0.4.0/kittycad/models/drawing_cmd_req_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_error.py` & `kittycad-0.4.0/kittycad/models/drawing_error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_outcome.py` & `kittycad-0.4.0/kittycad/models/drawing_outcome.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/drawing_outcomes.py` & `kittycad-0.4.0/kittycad/models/drawing_outcomes.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/email_authentication_form.py` & `kittycad-0.4.0/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/engine_metadata.py` & `kittycad-0.4.0/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/error.py` & `kittycad-0.4.0/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/executor_metadata.py` & `kittycad-0.4.0/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/extended_user.py` & `kittycad-0.4.0/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.0/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.0/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_conversion.py` & `kittycad-0.4.0/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_density.py` & `kittycad-0.4.0/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_export_format.py` & `kittycad-0.4.0/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_import_format.py` & `kittycad-0.4.0/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_mass.py` & `kittycad-0.4.0/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_surface_area.py` & `kittycad-0.4.0/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_system_metadata.py` & `kittycad-0.4.0/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/file_volume.py` & `kittycad-0.4.0/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/gateway.py` & `kittycad-0.4.0/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/index_info.py` & `kittycad-0.4.0/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/invoice.py` & `kittycad-0.4.0/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/invoice_line_item.py` & `kittycad-0.4.0/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/invoice_status.py` & `kittycad-0.4.0/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/jetstream.py` & `kittycad-0.4.0/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.0/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/jetstream_config.py` & `kittycad-0.4.0/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/jetstream_stats.py` & `kittycad-0.4.0/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/leaf_node.py` & `kittycad-0.4.0/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/mesh.py` & `kittycad-0.4.0/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.0/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/metadata.py` & `kittycad-0.4.0/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/method.py` & `kittycad-0.4.0/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/new_address.py` & `kittycad-0.4.0/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.0/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/onboarding.py` & `kittycad-0.4.0/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/output_file.py` & `kittycad-0.4.0/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/payment_intent.py` & `kittycad-0.4.0/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/payment_method.py` & `kittycad-0.4.0/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.0/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/physics_constant.py` & `kittycad-0.4.0/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/physics_constant_name.py` & `kittycad-0.4.0/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/plugins_info.py` & `kittycad-0.4.0/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/point_e_metadata.py` & `kittycad-0.4.0/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/pong.py` & `kittycad-0.4.0/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/registry_service_config.py` & `kittycad-0.4.0/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/runtime.py` & `kittycad-0.4.0/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/session.py` & `kittycad-0.4.0/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.0/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_acceleration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_acceleration_format.py` & `kittycad-0.4.0/kittycad/models/unit_acceleration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_angle_format.py` & `kittycad-0.4.0/kittycad/models/unit_angle_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_angular_velocity_format.py` & `kittycad-0.4.0/kittycad/models/unit_angular_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_area_format.py` & `kittycad-0.4.0/kittycad/models/unit_area_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_charge_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_charge_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_concentration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_concentration_format.py` & `kittycad-0.4.0/kittycad/models/unit_concentration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_data_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_data_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_data_format.py` & `kittycad-0.4.0/kittycad/models/unit_data_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_format.py` & `kittycad-0.4.0/kittycad/models/unit_data_transfer_rate_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_density_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_density_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_density_format.py` & `kittycad-0.4.0/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_energy_format.py` & `kittycad-0.4.0/kittycad/models/unit_energy_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_force_format.py` & `kittycad-0.4.0/kittycad/models/unit_force_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_illuminance_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_illuminance_format.py` & `kittycad-0.4.0/kittycad/models/unit_illuminance_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_length_format.py` & `kittycad-0.4.0/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_mass_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_mass_format.py` & `kittycad-0.4.0/kittycad/models/unit_mass_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_metric_power.py` & `kittycad-0.4.0/kittycad/models/unit_metric_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_metric_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_power_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_pressure_format.py` & `kittycad-0.4.0/kittycad/models/unit_pressure_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_radiation_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_radiation_format.py` & `kittycad-0.4.0/kittycad/models/unit_radiation_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_radioactivity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_radioactivity_format.py` & `kittycad-0.4.0/kittycad/models/unit_radioactivity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_solid_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_temperature_format.py` & `kittycad-0.4.0/kittycad/models/unit_temperature_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_time_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_time_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_time_format.py` & `kittycad-0.4.0/kittycad/models/unit_time_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_velocity_format.py` & `kittycad-0.4.0/kittycad/models/unit_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_voltage_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_volume_conversion.py` & `kittycad-0.4.0/kittycad/models/unit_volume_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/unit_volume_format.py` & `kittycad-0.4.0/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/update_user.py` & `kittycad-0.4.0/kittycad/models/update_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/user.py` & `kittycad-0.4.0/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/user_results_page.py` & `kittycad-0.4.0/kittycad/models/user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/models/verification_token.py` & `kittycad-0.4.0/kittycad/models/verification_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/kittycad/types.py` & `kittycad-0.4.0/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.9/pyproject.toml` & `kittycad-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.3.9"
+version = "0.4.0"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
@@ -20,27 +20,27 @@
 [tool.poetry.dev-dependencies]
 autoclasstoc = "^1.6.0"
 black = "^22.0.0"
 isort = "^5.12.0"
 jsonpatch = "^1.32"
 mypy = "^1.2.0"
 openapi-parser = "^0.2.6"
-openapi-spec-validator = "^0.4.0"
+openapi-spec-validator = "^0.5.6"
 prance = "^0.22.11"
 pyenchant = "^3.2.2"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.264"
-Sphinx = "^4.3.1"
-sphinx-autoapi = "^0.5.0"
+ruff = "^0.0.265"
+Sphinx = "^6.2.1"
+sphinx-autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-copybutton = "^0.5.2"
-sphinxext-opengraph = "^0.4.0"
+sphinxext-opengraph = "^0.8.2"
 sphinx-rtd-theme = "^1.0.0"
 toml = "^0.10.2"
 types-python-dateutil = "^2.8.0"
 types-toml = "^0.10.1"
 
 [build-system]
 requires = ["poetry>=1.0"]
@@ -87,15 +87,17 @@
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.per-file-ignores]
 # We exclude init files since otherwise ruff will delete all the unused imports.
 # This code comes from here: https://beta.ruff.rs/docs/rules/#pyflakes-f
 "__init__.py" = ["F401"]
+"examples_test.py" = ["F841"]
 
 [tool.mypy]
 exclude = []
 show_error_codes = true
 ignore_missing_imports = true
+check_untyped_defs = true
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
```

### Comparing `kittycad-0.3.9/PKG-INFO` & `kittycad-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.3.9
+Version: 0.4.0
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


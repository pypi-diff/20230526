# Comparing `tmp/kittycad-0.4.2.tar.gz` & `tmp/kittycad-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.4.2.tar", max compression
+gzip compressed data, was "kittycad-0.4.3.tar", max compression
```

## Comparing `kittycad-0.4.2.tar` & `kittycad-0.4.3.tar`

### file list

```diff
@@ -1,276 +1,230 @@
--rw-r--r--   0        0        0     1065 2023-05-23 21:26:44.314666 kittycad-0.4.2/LICENSE
--rw-r--r--   0        0        0      875 2023-05-23 21:26:44.314666 kittycad-0.4.2/README.md
--rw-r--r--   0        0        0       48 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3781 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3559 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3110 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2799 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3243 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6149 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4236 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     5005 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4815 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4351 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2879 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2784 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4284 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2911 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2338 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      161 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1781 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3195 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4635 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4461 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     5162 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     5290 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     4559 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     4487 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3220 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2139 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2383 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2629 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2564 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2193 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2245 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      144 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/__init__.py
--rw-r--r--   0        0        0     2794 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/cmd.py
--rw-r--r--   0        0        0     2701 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/cmd_batch.py
--rw-r--r--   0        0        0     1995 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/modeling_commands_ws.py
--rw-r--r--   0        0        0      123 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2956 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2638 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2431 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2655 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2681 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2616 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2684 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2954 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2483 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3966 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3784 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     4051 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3758 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     4082 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     4230 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3971 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3918 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3955 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3848 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3886 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3919 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2757 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3061 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3185 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2480 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2506 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2523 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2629 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4105 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4187 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2779 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/client.py
--rw-r--r--   0        0        0     5250 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/client_test.py
--rw-r--r--   0        0        0   129480 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/examples_test.py
--rw-r--r--   0        0        0     7966 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8574 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3455 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5909 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34857 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/customer.py
--rw-r--r--   0        0        0     4468 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1789 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      529 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     1940 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extrude.py
--rw-r--r--   0        0        0     5862 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6222 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5887 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5869 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5684 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5590 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     2007 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/line3d.py
--rw-r--r--   0        0        0     1337 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/method.py
--rw-r--r--   0        0        0     1726 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd.py
--rw-r--r--   0        0        0       76 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_id.py
--rw-r--r--   0        0        0     2456 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_req.py
--rw-r--r--   0        0        0     1752 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_req_batch.py
--rw-r--r--   0        0        0     2399 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_error.py
--rw-r--r--   0        0        0     1878 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_outcome.py
--rw-r--r--   0        0        0     1511 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_outcomes.py
--rw-r--r--   0        0        0     3081 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2509 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5586 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1530 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point2d.py
--rw-r--r--   0        0        0     1691 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point3d.py
--rw-r--r--   0        0        0     1498 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3855 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6479 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      642 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      916 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6522 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      754 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      888 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      380 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6492 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      752 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      539 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6539 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      656 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6414 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0     1488 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0     1162 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      645 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6466 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      584 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     2187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6604 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      402 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6483 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      389 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1094 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0     3438 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6421 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6449 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6459 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      468 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6427 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      725 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6440 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      586 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6492 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      570 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6457 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      500 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6466 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      674 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      902 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6427 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      753 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6414 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      452 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     3286 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2577 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/types.py
--rw-r--r--   0        0        0     2472 2023-05-23 21:26:45.194695 kittycad-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 19:40:36.890207 kittycad-0.4.3/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-26 19:40:36.890207 kittycad-0.4.3/README.md
+-rw-r--r--   0        0        0       48 2023-05-26 19:40:37.658231 kittycad-0.4.3/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3559 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3110 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2799 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3243 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6149 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4236 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5005 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4815 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4351 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2879 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2784 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4284 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2911 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2338 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      161 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3195 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     4635 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4461 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     5162 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     5290 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     4559 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     4487 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3220 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2139 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2383 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2629 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2564 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2193 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2245 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      144 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/__init__.py
+-rw-r--r--   0        0        0     2794 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/cmd.py
+-rw-r--r--   0        0        0     2701 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/cmd_batch.py
+-rw-r--r--   0        0        0     1995 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/modeling_commands_ws.py
+-rw-r--r--   0        0        0      123 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2956 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2638 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2431 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2655 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2681 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2616 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2684 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2954 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2483 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3679 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3653 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3729 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_current_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3677 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_frequency_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3651 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3677 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3755 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3833 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_torque_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2757 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3061 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3185 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2480 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2506 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2523 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2629 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4105 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4187 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2779 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/client.py
+-rw-r--r--   0        0        0     5250 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/client_test.py
+-rw-r--r--   0        0        0    99150 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/examples_test.py
+-rw-r--r--   0        0        0     5856 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8574 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3455 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5909 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34857 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4468 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1789 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      529 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     1940 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extrude.py
+-rw-r--r--   0        0        0     5862 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6222 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5887 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5869 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5684 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5590 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     2007 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/line3d.py
+-rw-r--r--   0        0        0     1337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/method.py
+-rw-r--r--   0        0        0     1726 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd.py
+-rw-r--r--   0        0        0       76 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_id.py
+-rw-r--r--   0        0        0     2456 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_req.py
+-rw-r--r--   0        0        0     1752 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_req_batch.py
+-rw-r--r--   0        0        0     2399 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_error.py
+-rw-r--r--   0        0        0     1878 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_outcome.py
+-rw-r--r--   0        0        0     1511 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_outcomes.py
+-rw-r--r--   0        0        0     3081 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2509 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5586 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1530 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point2d.py
+-rw-r--r--   0        0        0     1691 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point3d.py
+-rw-r--r--   0        0        0     1498 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3855 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0      377 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_angle.py
+-rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0     1937 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_area.py
+-rw-r--r--   0        0        0     6311 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      623 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_current.py
+-rw-r--r--   0        0        0     6350 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_current_conversion.py
+-rw-r--r--   0        0        0      934 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_energy.py
+-rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_force.py
+-rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      997 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_frequency.py
+-rw-r--r--   0        0        0     6376 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_frequency_conversion.py
+-rw-r--r--   0        0        0     1522 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_length.py
+-rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     1754 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_mass.py
+-rw-r--r--   0        0        0     6311 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1014 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_power.py
+-rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      973 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_pressure.py
+-rw-r--r--   0        0        0     6363 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      593 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_temperature.py
+-rw-r--r--   0        0        0     6402 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      415 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_torque.py
+-rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_torque_conversion.py
+-rw-r--r--   0        0        0     2355 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_volume.py
+-rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     2577 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/types.py
+-rw-r--r--   0        0        0     2472 2023-05-26 19:40:37.670232 kittycad-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.3/PKG-INFO
```

### Comparing `kittycad-0.4.2/LICENSE` & `kittycad-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/README.md` & `kittycad-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.3/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.3/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.3/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.3/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.3/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.3/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.3/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.3/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.3/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.3/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.3/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.3/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.3/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.3/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.3/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.3/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.3/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.3/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.3/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.3/kittycad/api/executor/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.3/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.3/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.3/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_density.py` & `kittycad-0.4.3/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_mass.py` & `kittycad-0.4.3/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.3/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/create_file_volume.py` & `kittycad-0.4.3/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.3/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.3/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.3/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/hidden/logout.py` & `kittycad-0.4.3/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.3/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.3/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.3/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/meta/get_schema.py` & `kittycad-0.4.3/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/meta/ping.py` & `kittycad-0.4.3/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/modeling/cmd.py` & `kittycad-0.4.3/kittycad/api/modeling/cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/modeling/cmd_batch.py` & `kittycad-0.4.3/kittycad/api/modeling/cmd_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/modeling/modeling_commands_ws.py` & `kittycad-0.4.3/kittycad/api/modeling/modeling_commands_ws.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.3/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_acceleration_conversion import UnitAccelerationConversion
-from ...models.unit_acceleration_format import UnitAccelerationFormat
+from ...models.unit_temperature import UnitTemperature
+from ...models.unit_temperature_conversion import UnitTemperatureConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAccelerationFormat,
-    src_format: UnitAccelerationFormat,
+    input_unit: UnitTemperature,
+    output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/acceleration/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/temperature/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitAccelerationConversion, Error]]:
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitAccelerationConversion.from_dict(response.json())
+        response_200 = UnitTemperatureConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitAccelerationFormat,
-    src_format: UnitAccelerationFormat,
+    input_unit: UnitTemperature,
+    output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAccelerationFormat,
-    src_format: UnitAccelerationFormat,
+    input_unit: UnitTemperature,
+    output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAccelerationConversion, Error]]:
-    """Convert an acceleration unit value to another acceleration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
+    """Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAccelerationFormat,
-    src_format: UnitAccelerationFormat,
+    input_unit: UnitTemperature,
+    output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAccelerationConversion, Error]]]:
+) -> Response[Optional[Union[UnitTemperatureConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAccelerationFormat,
-    src_format: UnitAccelerationFormat,
+    input_unit: UnitTemperature,
+    output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAccelerationConversion, Error]]:
-    """Convert an acceleration unit value to another acceleration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitTemperatureConversion, Error]]:
+    """Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_angle_conversion import UnitAngleConversion
-from ...models.unit_angle_format import UnitAngleFormat
+from ...models.unit_energy import UnitEnergy
+from ...models.unit_energy_conversion import UnitEnergyConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    input_unit: UnitEnergy,
+    output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/angle/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/energy/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitAngleConversion, Error]]:
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
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
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
+    input_unit: UnitEnergy,
+    output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
+) -> Response[Optional[Union[UnitEnergyConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    input_unit: UnitEnergy,
+    output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAngleConversion, Error]]:
-    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitEnergyConversion, Error]]:
+    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    input_unit: UnitEnergy,
+    output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
+) -> Response[Optional[Union[UnitEnergyConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAngleFormat,
-    src_format: UnitAngleFormat,
+    input_unit: UnitEnergy,
+    output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAngleConversion, Error]]:
-    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitEnergyConversion, Error]]:
+    """Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_angular_velocity_conversion import UnitAngularVelocityConversion
-from ...models.unit_angular_velocity_format import UnitAngularVelocityFormat
+from ...models.unit_area import UnitArea
+from ...models.unit_area_conversion import UnitAreaConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAngularVelocityFormat,
-    src_format: UnitAngularVelocityFormat,
+    input_unit: UnitArea,
+    output_unit: UnitArea,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/angular-velocity/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/area/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
+) -> Optional[Union[UnitAreaConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitAngularVelocityConversion.from_dict(response.json())
+        response_200 = UnitAreaConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitAngularVelocityFormat,
-    src_format: UnitAngularVelocityFormat,
+    input_unit: UnitArea,
+    output_unit: UnitArea,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAngularVelocityFormat,
-    src_format: UnitAngularVelocityFormat,
+    input_unit: UnitArea,
+    output_unit: UnitArea,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
-    """Convert an angular velocity unit value to another angular velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAreaConversion, Error]]:
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAngularVelocityFormat,
-    src_format: UnitAngularVelocityFormat,
+    input_unit: UnitArea,
+    output_unit: UnitArea,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAngularVelocityConversion, Error]]]:
+) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAngularVelocityFormat,
-    src_format: UnitAngularVelocityFormat,
+    input_unit: UnitArea,
+    output_unit: UnitArea,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAngularVelocityConversion, Error]]:
-    """Convert an angular velocity unit value to another angular velocity unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAreaConversion, Error]]:
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_area_conversion import UnitAreaConversion
-from ...models.unit_area_format import UnitAreaFormat
+from ...models.unit_angle import UnitAngle
+from ...models.unit_angle_conversion import UnitAngleConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    input_unit: UnitAngle,
+    output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/area/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/angle/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitAreaConversion, Error]]:
+) -> Optional[Union[UnitAngleConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitAreaConversion.from_dict(response.json())
+        response_200 = UnitAngleConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    input_unit: UnitAngle,
+    output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    input_unit: UnitAngle,
+    output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAreaConversion, Error]]:
-    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    input_unit: UnitAngle,
+    output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitAreaConversion, Error]]]:
+) -> Response[Optional[Union[UnitAngleConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitAreaFormat,
-    src_format: UnitAreaFormat,
+    input_unit: UnitAngle,
+    output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitAreaConversion, Error]]:
-    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_frequency_unit_conversion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_charge_conversion import UnitChargeConversion
-from ...models.unit_charge_format import UnitChargeFormat
+from ...models.unit_frequency import UnitFrequency
+from ...models.unit_frequency_conversion import UnitFrequencyConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitChargeFormat,
-    src_format: UnitChargeFormat,
+    input_unit: UnitFrequency,
+    output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/charge/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/frequency/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitChargeConversion, Error]]:
+) -> Optional[Union[UnitFrequencyConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitChargeConversion.from_dict(response.json())
+        response_200 = UnitFrequencyConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
+) -> Response[Optional[Union[UnitFrequencyConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitChargeFormat,
-    src_format: UnitChargeFormat,
+    input_unit: UnitFrequency,
+    output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
+) -> Response[Optional[Union[UnitFrequencyConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitChargeFormat,
-    src_format: UnitChargeFormat,
+    input_unit: UnitFrequency,
+    output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitChargeConversion, Error]]:
-    """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitFrequencyConversion, Error]]:
+    """Convert a frequency unit value to another frequency unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitChargeFormat,
-    src_format: UnitChargeFormat,
+    input_unit: UnitFrequency,
+    output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitChargeConversion, Error]]]:
+) -> Response[Optional[Union[UnitFrequencyConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitChargeFormat,
-    src_format: UnitChargeFormat,
+    input_unit: UnitFrequency,
+    output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitChargeConversion, Error]]:
-    """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitFrequencyConversion, Error]]:
+    """Convert a frequency unit value to another frequency unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_concentration_conversion import UnitConcentrationConversion
-from ...models.unit_concentration_format import UnitConcentrationFormat
+from ...models.unit_force import UnitForce
+from ...models.unit_force_conversion import UnitForceConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitConcentrationFormat,
-    src_format: UnitConcentrationFormat,
+    input_unit: UnitForce,
+    output_unit: UnitForce,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/concentration/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/force/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitConcentrationConversion, Error]]:
+) -> Optional[Union[UnitForceConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitConcentrationConversion.from_dict(response.json())
+        response_200 = UnitForceConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitConcentrationFormat,
-    src_format: UnitConcentrationFormat,
+    input_unit: UnitForce,
+    output_unit: UnitForce,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitConcentrationFormat,
-    src_format: UnitConcentrationFormat,
+    input_unit: UnitForce,
+    output_unit: UnitForce,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitConcentrationConversion, Error]]:
-    """Convert a concentration unit value to another concentration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitForceConversion, Error]]:
+    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitConcentrationFormat,
-    src_format: UnitConcentrationFormat,
+    input_unit: UnitForce,
+    output_unit: UnitForce,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitConcentrationConversion, Error]]]:
+) -> Response[Optional[Union[UnitForceConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitConcentrationFormat,
-    src_format: UnitConcentrationFormat,
+    input_unit: UnitForce,
+    output_unit: UnitForce,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitConcentrationConversion, Error]]:
-    """Convert a concentration unit value to another concentration unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitForceConversion, Error]]:
+    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_data_conversion import UnitDataConversion
-from ...models.unit_data_format import UnitDataFormat
+from ...models.unit_pressure import UnitPressure
+from ...models.unit_pressure_conversion import UnitPressureConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    input_unit: UnitPressure,
+    output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/data/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/pressure/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitDataConversion, Error]]:
+) -> Optional[Union[UnitPressureConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitDataConversion.from_dict(response.json())
+        response_200 = UnitPressureConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitDataConversion, Error]]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    input_unit: UnitPressure,
+    output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitDataConversion, Error]]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    input_unit: UnitPressure,
+    output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitDataConversion, Error]]:
-    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitPressureConversion, Error]]:
+    """Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    input_unit: UnitPressure,
+    output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitDataConversion, Error]]]:
+) -> Response[Optional[Union[UnitPressureConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitDataFormat,
-    src_format: UnitDataFormat,
+    input_unit: UnitPressure,
+    output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitDataConversion, Error]]:
-    """Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitPressureConversion, Error]]:
+    """Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_density_conversion import UnitDensityConversion
-from ...models.unit_density_format import UnitDensityFormat
+from ...models.unit_volume import UnitVolume
+from ...models.unit_volume_conversion import UnitVolumeConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    input_unit: UnitVolume,
+    output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/density/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/volume/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitDensityConversion, Error]]:
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
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
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
+    input_unit: UnitVolume,
+    output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
+) -> Response[Optional[Union[UnitVolumeConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    input_unit: UnitVolume,
+    output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitDensityConversion, Error]]:
-    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVolumeConversion, Error]]:
+    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    input_unit: UnitVolume,
+    output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitDensityConversion, Error]]]:
+) -> Response[Optional[Union[UnitVolumeConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitDensityFormat,
-    src_format: UnitDensityFormat,
+    input_unit: UnitVolume,
+    output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitDensityConversion, Error]]:
-    """Convert a density unit value to another density unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitVolumeConversion, Error]]:
+    """Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_torque_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_force_conversion import UnitForceConversion
-from ...models.unit_force_format import UnitForceFormat
+from ...models.unit_torque import UnitTorque
+from ...models.unit_torque_conversion import UnitTorqueConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitForceFormat,
-    src_format: UnitForceFormat,
+    input_unit: UnitTorque,
+    output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/force/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/torque/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitForceConversion, Error]]:
+) -> Optional[Union[UnitTorqueConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitForceConversion.from_dict(response.json())
+        response_200 = UnitTorqueConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitForceConversion, Error]]]:
+) -> Response[Optional[Union[UnitTorqueConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitForceFormat,
-    src_format: UnitForceFormat,
+    input_unit: UnitTorque,
+    output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitForceConversion, Error]]]:
+) -> Response[Optional[Union[UnitTorqueConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitForceFormat,
-    src_format: UnitForceFormat,
+    input_unit: UnitTorque,
+    output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitForceConversion, Error]]:
-    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitTorqueConversion, Error]]:
+    """Convert a torque unit value to another torque unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitForceFormat,
-    src_format: UnitForceFormat,
+    input_unit: UnitTorque,
+    output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitForceConversion, Error]]]:
+) -> Response[Optional[Union[UnitTorqueConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitForceFormat,
-    src_format: UnitForceFormat,
+    input_unit: UnitTorque,
+    output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitForceConversion, Error]]:
-    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitTorqueConversion, Error]]:
+    """Convert a torque unit value to another torque unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_illuminance_conversion import UnitIlluminanceConversion
-from ...models.unit_illuminance_format import UnitIlluminanceFormat
+from ...models.unit_length import UnitLength
+from ...models.unit_length_conversion import UnitLengthConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitIlluminanceFormat,
-    src_format: UnitIlluminanceFormat,
+    input_unit: UnitLength,
+    output_unit: UnitLength,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/illuminance/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/length/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitIlluminanceConversion, Error]]:
+) -> Optional[Union[UnitLengthConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitIlluminanceConversion.from_dict(response.json())
+        response_200 = UnitLengthConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitIlluminanceFormat,
-    src_format: UnitIlluminanceFormat,
+    input_unit: UnitLength,
+    output_unit: UnitLength,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitIlluminanceFormat,
-    src_format: UnitIlluminanceFormat,
+    input_unit: UnitLength,
+    output_unit: UnitLength,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitIlluminanceConversion, Error]]:
-    """Convert a illuminance unit value to another illuminance unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitLengthConversion, Error]]:
+    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitIlluminanceFormat,
-    src_format: UnitIlluminanceFormat,
+    input_unit: UnitLength,
+    output_unit: UnitLength,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitIlluminanceConversion, Error]]]:
+) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitIlluminanceFormat,
-    src_format: UnitIlluminanceFormat,
+    input_unit: UnitLength,
+    output_unit: UnitLength,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitIlluminanceConversion, Error]]:
-    """Convert a illuminance unit value to another illuminance unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitLengthConversion, Error]]:
+    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_length_conversion import UnitLengthConversion
-from ...models.unit_length_format import UnitLengthFormat
+from ...models.unit_mass import UnitMass
+from ...models.unit_mass_conversion import UnitMassConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitLengthFormat,
-    src_format: UnitLengthFormat,
+    input_unit: UnitMass,
+    output_unit: UnitMass,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/length/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/mass/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitLengthConversion, Error]]:
+) -> Optional[Union[UnitMassConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitLengthConversion.from_dict(response.json())
+        response_200 = UnitMassConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitLengthFormat,
-    src_format: UnitLengthFormat,
+    input_unit: UnitMass,
+    output_unit: UnitMass,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitLengthFormat,
-    src_format: UnitLengthFormat,
+    input_unit: UnitMass,
+    output_unit: UnitMass,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitLengthConversion, Error]]:
-    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitMassConversion, Error]]:
+    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitLengthFormat,
-    src_format: UnitLengthFormat,
+    input_unit: UnitMass,
+    output_unit: UnitMass,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitLengthConversion, Error]]]:
+) -> Response[Optional[Union[UnitMassConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitLengthFormat,
-    src_format: UnitLengthFormat,
+    input_unit: UnitMass,
+    output_unit: UnitMass,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitLengthConversion, Error]]:
-    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitMassConversion, Error]]:
+    """Convert a mass unit value to another mass unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power_cubed_conversion import UnitMetricPowerCubedConversion
+from ...models.unit_power import UnitPower
+from ...models.unit_power_conversion import UnitPowerConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitPower,
+    output_unit: UnitPower,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/metric/cubed/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/power/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -34,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
+) -> Optional[Union[UnitPowerConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
+        response_200 = UnitPowerConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitPower,
+    output_unit: UnitPower,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitPower,
+    output_unit: UnitPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
-    """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitPowerConversion, Error]]:
+    """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitPower,
+    output_unit: UnitPower,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitMetricPowerCubedConversion, Error]]]:
+) -> Response[Optional[Union[UnitPowerConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitPower,
+    output_unit: UnitPower,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitMetricPowerCubedConversion, Error]]:
-    """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitPowerConversion, Error]]:
+    """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.4.3/kittycad/api/unit/get_current_unit_conversion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power_squared_conversion import (
-    UnitMetricPowerSquaredConversion,
-)
+from ...models.unit_current import UnitCurrent
+from ...models.unit_current_conversion import UnitCurrentConversion
 from ...types import Response
 
 
 def _get_kwargs(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitCurrent,
+    output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/unit/conversion/metric/squared/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+    url = "{}/unit/conversion/current/{input_unit}/{output_unit}".format(
+        client.base_url, input_unit=input_unit, output_unit=output_unit
     )  # noqa: E501
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
@@ -36,107 +34,107 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
+) -> Optional[Union[UnitCurrentConversion, Error]]:
     if response.status_code == 200:
-        response_200 = UnitMetricPowerSquaredConversion.from_dict(response.json())
+        response_200 = UnitCurrentConversion.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
+) -> Response[Optional[Union[UnitCurrentConversion, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitCurrent,
+    output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
+) -> Response[Optional[Union[UnitCurrentConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitCurrent,
+    output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
-    """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitCurrentConversion, Error]]:
+    """Convert a current unit value to another current unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return sync_detailed(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitCurrent,
+    output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
-) -> Response[Optional[Union[UnitMetricPowerSquaredConversion, Error]]]:
+) -> Response[Optional[Union[UnitCurrentConversion, Error]]]:
     kwargs = _get_kwargs(
-        output_format=output_format,
-        src_format=src_format,
+        input_unit=input_unit,
+        output_unit=output_unit,
         value=value,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    output_format: UnitMetricPower,
-    src_format: UnitMetricPower,
+    input_unit: UnitCurrent,
+    output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
-) -> Optional[Union[UnitMetricPowerSquaredConversion, Error]]:
-    """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+) -> Optional[Union[UnitCurrentConversion, Error]]:
+    """Convert a current unit value to another current unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            output_format=output_format,
-            src_format=src_format,
+            input_unit=input_unit,
+            output_unit=output_unit,
             value=value,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.2/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.3/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.3/kittycad/api/users/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user.py` & `kittycad-0.4.3/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.3/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.3/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.4.3/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user_self.py` & `kittycad-0.4.3/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.4.3/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/list_users.py` & `kittycad-0.4.3/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/list_users_extended.py` & `kittycad-0.4.3/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/api/users/update_user_self.py` & `kittycad-0.4.3/kittycad/api/users/update_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/client.py` & `kittycad-0.4.3/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/client_test.py` & `kittycad-0.4.3/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/examples_test.py` & `kittycad-0.4.3/kittycad/examples_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,42 +53,26 @@
     get_payment_information_for_user,
     list_invoices_for_user,
     list_payment_methods_for_user,
     update_payment_information_for_user,
     validate_customer_tax_information_for_user,
 )
 from kittycad.api.unit import (
-    get_acceleration_unit_conversion,
     get_angle_unit_conversion,
-    get_angular_velocity_unit_conversion,
     get_area_unit_conversion,
-    get_charge_unit_conversion,
-    get_concentration_unit_conversion,
-    get_data_transfer_rate_unit_conversion,
-    get_data_unit_conversion,
-    get_density_unit_conversion,
+    get_current_unit_conversion,
     get_energy_unit_conversion,
     get_force_unit_conversion,
-    get_illuminance_unit_conversion,
+    get_frequency_unit_conversion,
     get_length_unit_conversion,
-    get_magnetic_field_strength_unit_conversion,
-    get_magnetic_flux_unit_conversion,
     get_mass_unit_conversion,
-    get_metric_power_cubed_unit_conversion,
-    get_metric_power_squared_unit_conversion,
-    get_metric_power_unit_conversion,
     get_power_unit_conversion,
     get_pressure_unit_conversion,
-    get_radiation_unit_conversion,
-    get_radioactivity_unit_conversion,
-    get_solid_angle_unit_conversion,
     get_temperature_unit_conversion,
-    get_time_unit_conversion,
-    get_velocity_unit_conversion,
-    get_voltage_unit_conversion,
+    get_torque_unit_conversion,
     get_volume_unit_conversion,
 )
 from kittycad.api.users import (
     delete_user_self,
     get_session_for_user,
     get_user,
     get_user_extended,
@@ -128,42 +112,26 @@
     ModelingOutcomes,
     Onboarding,
     PaymentIntent,
     PaymentMethod,
     PhysicsConstant,
     Pong,
     Session,
-    UnitAccelerationConversion,
     UnitAngleConversion,
-    UnitAngularVelocityConversion,
     UnitAreaConversion,
-    UnitChargeConversion,
-    UnitConcentrationConversion,
-    UnitDataConversion,
-    UnitDataTransferRateConversion,
-    UnitDensityConversion,
+    UnitCurrentConversion,
     UnitEnergyConversion,
     UnitForceConversion,
-    UnitIlluminanceConversion,
+    UnitFrequencyConversion,
     UnitLengthConversion,
-    UnitMagneticFieldStrengthConversion,
-    UnitMagneticFluxConversion,
     UnitMassConversion,
-    UnitMetricPowerConversion,
-    UnitMetricPowerCubedConversion,
-    UnitMetricPowerSquaredConversion,
     UnitPowerConversion,
     UnitPressureConversion,
-    UnitRadiationConversion,
-    UnitRadioactivityConversion,
-    UnitSolidAngleConversion,
     UnitTemperatureConversion,
-    UnitTimeConversion,
-    UnitVelocityConversion,
-    UnitVoltageConversion,
+    UnitTorqueConversion,
     UnitVolumeConversion,
     User,
     UserResultsPage,
     VerificationToken,
 )
 from kittycad.models.api_call_query_group_by import ApiCallQueryGroupBy
 from kittycad.models.api_call_status import ApiCallStatus
@@ -176,43 +144,27 @@
 from kittycad.models.image_type import ImageType
 from kittycad.models.line3d import Line3d
 from kittycad.models.modeling_cmd_id import ModelingCmdId
 from kittycad.models.modeling_cmd_req import ModelingCmdReq
 from kittycad.models.modeling_cmd_req_batch import ModelingCmdReqBatch
 from kittycad.models.physics_constant_name import PhysicsConstantName
 from kittycad.models.point3d import Point3d
-from kittycad.models.unit_acceleration_format import UnitAccelerationFormat
-from kittycad.models.unit_angle_format import UnitAngleFormat
-from kittycad.models.unit_angular_velocity_format import UnitAngularVelocityFormat
-from kittycad.models.unit_area_format import UnitAreaFormat
-from kittycad.models.unit_charge_format import UnitChargeFormat
-from kittycad.models.unit_concentration_format import UnitConcentrationFormat
-from kittycad.models.unit_data_format import UnitDataFormat
-from kittycad.models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
-from kittycad.models.unit_density_format import UnitDensityFormat
-from kittycad.models.unit_energy_format import UnitEnergyFormat
-from kittycad.models.unit_force_format import UnitForceFormat
-from kittycad.models.unit_illuminance_format import UnitIlluminanceFormat
-from kittycad.models.unit_length_format import UnitLengthFormat
-from kittycad.models.unit_magnetic_field_strength_format import (
-    UnitMagneticFieldStrengthFormat,
-)
-from kittycad.models.unit_magnetic_flux_format import UnitMagneticFluxFormat
-from kittycad.models.unit_mass_format import UnitMassFormat
-from kittycad.models.unit_metric_power import UnitMetricPower
-from kittycad.models.unit_power_format import UnitPowerFormat
-from kittycad.models.unit_pressure_format import UnitPressureFormat
-from kittycad.models.unit_radiation_format import UnitRadiationFormat
-from kittycad.models.unit_radioactivity_format import UnitRadioactivityFormat
-from kittycad.models.unit_solid_angle_format import UnitSolidAngleFormat
-from kittycad.models.unit_temperature_format import UnitTemperatureFormat
-from kittycad.models.unit_time_format import UnitTimeFormat
-from kittycad.models.unit_velocity_format import UnitVelocityFormat
-from kittycad.models.unit_voltage_format import UnitVoltageFormat
-from kittycad.models.unit_volume_format import UnitVolumeFormat
+from kittycad.models.unit_angle import UnitAngle
+from kittycad.models.unit_area import UnitArea
+from kittycad.models.unit_current import UnitCurrent
+from kittycad.models.unit_energy import UnitEnergy
+from kittycad.models.unit_force import UnitForce
+from kittycad.models.unit_frequency import UnitFrequency
+from kittycad.models.unit_length import UnitLength
+from kittycad.models.unit_mass import UnitMass
+from kittycad.models.unit_power import UnitPower
+from kittycad.models.unit_pressure import UnitPressure
+from kittycad.models.unit_temperature import UnitTemperature
+from kittycad.models.unit_torque import UnitTorque
+from kittycad.models.unit_volume import UnitVolume
 from kittycad.models.update_user import UpdateUser
 from kittycad.types import Response
 
 
 @pytest.mark.skip
 def test_get_schema():
     # Create our client.
@@ -1734,83 +1686,24 @@
     # OR run async with more info
     response: Response[Optional[Union[Pong, Error]]] = await ping.asyncio_detailed(
         client=client,
     )
 
 
 @pytest.mark.skip
-def test_get_acceleration_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitAccelerationConversion, Error]
-    ] = get_acceleration_unit_conversion.sync(
-        client=client,
-        output_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        src_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitAccelerationConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitAccelerationConversion, Error]]
-    ] = get_acceleration_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        src_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_acceleration_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitAccelerationConversion, Error]
-    ] = await get_acceleration_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        src_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitAccelerationConversion, Error]]
-    ] = await get_acceleration_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        src_format=UnitAccelerationFormat.METERS_PER_SECOND_SQUARED,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
 def test_get_angle_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitAngleConversion, Error]
     ] = get_angle_unit_conversion.sync(
         client=client,
-        output_format=UnitAngleFormat.RADIAN,
-        src_format=UnitAngleFormat.RADIAN,
+        input_unit=UnitAngle.DEGREES,
+        output_unit=UnitAngle.DEGREES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -1818,16 +1711,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitAngleConversion, Error]]
     ] = get_angle_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitAngleFormat.RADIAN,
-        src_format=UnitAngleFormat.RADIAN,
+        input_unit=UnitAngle.DEGREES,
+        output_unit=UnitAngle.DEGREES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -1835,98 +1728,39 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitAngleConversion, Error]
     ] = await get_angle_unit_conversion.asyncio(
         client=client,
-        output_format=UnitAngleFormat.RADIAN,
-        src_format=UnitAngleFormat.RADIAN,
+        input_unit=UnitAngle.DEGREES,
+        output_unit=UnitAngle.DEGREES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitAngleConversion, Error]]
     ] = await get_angle_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitAngleFormat.RADIAN,
-        src_format=UnitAngleFormat.RADIAN,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_angular_velocity_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitAngularVelocityConversion, Error]
-    ] = get_angular_velocity_unit_conversion.sync(
-        client=client,
-        output_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        src_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitAngularVelocityConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitAngularVelocityConversion, Error]]
-    ] = get_angular_velocity_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        src_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_angular_velocity_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitAngularVelocityConversion, Error]
-    ] = await get_angular_velocity_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        src_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitAngularVelocityConversion, Error]]
-    ] = await get_angular_velocity_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
-        src_format=UnitAngularVelocityFormat.RADIANS_PER_SECOND,
+        input_unit=UnitAngle.DEGREES,
+        output_unit=UnitAngle.DEGREES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_area_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[UnitAreaConversion, Error]] = get_area_unit_conversion.sync(
         client=client,
-        output_format=UnitAreaFormat.SQUARE_METER,
-        src_format=UnitAreaFormat.SQUARE_METER,
+        input_unit=UnitArea.ACRES,
+        output_unit=UnitArea.ACRES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -1934,16 +1768,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitAreaConversion, Error]]
     ] = get_area_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitAreaFormat.SQUARE_METER,
-        src_format=UnitAreaFormat.SQUARE_METER,
+        input_unit=UnitArea.ACRES,
+        output_unit=UnitArea.ACRES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -1951,334 +1785,100 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitAreaConversion, Error]
     ] = await get_area_unit_conversion.asyncio(
         client=client,
-        output_format=UnitAreaFormat.SQUARE_METER,
-        src_format=UnitAreaFormat.SQUARE_METER,
+        input_unit=UnitArea.ACRES,
+        output_unit=UnitArea.ACRES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitAreaConversion, Error]]
     ] = await get_area_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitAreaFormat.SQUARE_METER,
-        src_format=UnitAreaFormat.SQUARE_METER,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_charge_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitChargeConversion, Error]
-    ] = get_charge_unit_conversion.sync(
-        client=client,
-        output_format=UnitChargeFormat.COULOMB,
-        src_format=UnitChargeFormat.COULOMB,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitChargeConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitChargeConversion, Error]]
-    ] = get_charge_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitChargeFormat.COULOMB,
-        src_format=UnitChargeFormat.COULOMB,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_charge_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitChargeConversion, Error]
-    ] = await get_charge_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitChargeFormat.COULOMB,
-        src_format=UnitChargeFormat.COULOMB,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitChargeConversion, Error]]
-    ] = await get_charge_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitChargeFormat.COULOMB,
-        src_format=UnitChargeFormat.COULOMB,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_concentration_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitConcentrationConversion, Error]
-    ] = get_concentration_unit_conversion.sync(
-        client=client,
-        output_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        src_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitConcentrationConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitConcentrationConversion, Error]]
-    ] = get_concentration_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        src_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_concentration_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitConcentrationConversion, Error]
-    ] = await get_concentration_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        src_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitConcentrationConversion, Error]]
-    ] = await get_concentration_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        src_format=UnitConcentrationFormat.PARTS_PER_MILLION,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_data_transfer_rate_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitDataTransferRateConversion, Error]
-    ] = get_data_transfer_rate_unit_conversion.sync(
-        client=client,
-        output_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        src_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitDataTransferRateConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitDataTransferRateConversion, Error]]
-    ] = get_data_transfer_rate_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        src_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_data_transfer_rate_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitDataTransferRateConversion, Error]
-    ] = await get_data_transfer_rate_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        src_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitDataTransferRateConversion, Error]]
-    ] = await get_data_transfer_rate_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        src_format=UnitDataTransferRateFormat.BYTES_PER_SECOND,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_data_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[Union[UnitDataConversion, Error]] = get_data_unit_conversion.sync(
-        client=client,
-        output_format=UnitDataFormat.BYTE,
-        src_format=UnitDataFormat.BYTE,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitDataConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitDataConversion, Error]]
-    ] = get_data_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitDataFormat.BYTE,
-        src_format=UnitDataFormat.BYTE,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_data_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitDataConversion, Error]
-    ] = await get_data_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitDataFormat.BYTE,
-        src_format=UnitDataFormat.BYTE,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitDataConversion, Error]]
-    ] = await get_data_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitDataFormat.BYTE,
-        src_format=UnitDataFormat.BYTE,
+        input_unit=UnitArea.ACRES,
+        output_unit=UnitArea.ACRES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
-def test_get_density_unit_conversion():
+def test_get_current_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitDensityConversion, Error]
-    ] = get_density_unit_conversion.sync(
+        Union[UnitCurrentConversion, Error]
+    ] = get_current_unit_conversion.sync(
         client=client,
-        output_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
-        src_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
+        input_unit=UnitCurrent.AMPERES,
+        output_unit=UnitCurrent.AMPERES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
-    body: UnitDensityConversion = result
+    body: UnitCurrentConversion = result
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
-        Optional[Union[UnitDensityConversion, Error]]
-    ] = get_density_unit_conversion.sync_detailed(
+        Optional[Union[UnitCurrentConversion, Error]]
+    ] = get_current_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
-        src_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
+        input_unit=UnitCurrent.AMPERES,
+        output_unit=UnitCurrent.AMPERES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
-async def test_get_density_unit_conversion_async():
+async def test_get_current_unit_conversion_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitDensityConversion, Error]
-    ] = await get_density_unit_conversion.asyncio(
+        Union[UnitCurrentConversion, Error]
+    ] = await get_current_unit_conversion.asyncio(
         client=client,
-        output_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
-        src_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
+        input_unit=UnitCurrent.AMPERES,
+        output_unit=UnitCurrent.AMPERES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
-        Optional[Union[UnitDensityConversion, Error]]
-    ] = await get_density_unit_conversion.asyncio_detailed(
+        Optional[Union[UnitCurrentConversion, Error]]
+    ] = await get_current_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
-        src_format=UnitDensityFormat.KILOGRAMS_PER_CUBIC_METER,
+        input_unit=UnitCurrent.AMPERES,
+        output_unit=UnitCurrent.AMPERES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_energy_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitEnergyConversion, Error]
     ] = get_energy_unit_conversion.sync(
         client=client,
-        output_format=UnitEnergyFormat.JOULE,
-        src_format=UnitEnergyFormat.JOULE,
+        input_unit=UnitEnergy.BTU,
+        output_unit=UnitEnergy.BTU,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2286,16 +1886,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitEnergyConversion, Error]]
     ] = get_energy_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitEnergyFormat.JOULE,
-        src_format=UnitEnergyFormat.JOULE,
+        input_unit=UnitEnergy.BTU,
+        output_unit=UnitEnergy.BTU,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2303,41 +1903,41 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitEnergyConversion, Error]
     ] = await get_energy_unit_conversion.asyncio(
         client=client,
-        output_format=UnitEnergyFormat.JOULE,
-        src_format=UnitEnergyFormat.JOULE,
+        input_unit=UnitEnergy.BTU,
+        output_unit=UnitEnergy.BTU,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitEnergyConversion, Error]]
     ] = await get_energy_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitEnergyFormat.JOULE,
-        src_format=UnitEnergyFormat.JOULE,
+        input_unit=UnitEnergy.BTU,
+        output_unit=UnitEnergy.BTU,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_force_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitForceConversion, Error]
     ] = get_force_unit_conversion.sync(
         client=client,
-        output_format=UnitForceFormat.NEWTON,
-        src_format=UnitForceFormat.NEWTON,
+        input_unit=UnitForce.DYNES,
+        output_unit=UnitForce.DYNES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2345,16 +1945,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitForceConversion, Error]]
     ] = get_force_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitForceFormat.NEWTON,
-        src_format=UnitForceFormat.NEWTON,
+        input_unit=UnitForce.DYNES,
+        output_unit=UnitForce.DYNES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2362,100 +1962,100 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitForceConversion, Error]
     ] = await get_force_unit_conversion.asyncio(
         client=client,
-        output_format=UnitForceFormat.NEWTON,
-        src_format=UnitForceFormat.NEWTON,
+        input_unit=UnitForce.DYNES,
+        output_unit=UnitForce.DYNES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitForceConversion, Error]]
     ] = await get_force_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitForceFormat.NEWTON,
-        src_format=UnitForceFormat.NEWTON,
+        input_unit=UnitForce.DYNES,
+        output_unit=UnitForce.DYNES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
-def test_get_illuminance_unit_conversion():
+def test_get_frequency_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitIlluminanceConversion, Error]
-    ] = get_illuminance_unit_conversion.sync(
+        Union[UnitFrequencyConversion, Error]
+    ] = get_frequency_unit_conversion.sync(
         client=client,
-        output_format=UnitIlluminanceFormat.LUX,
-        src_format=UnitIlluminanceFormat.LUX,
+        input_unit=UnitFrequency.GIGAHERTZ,
+        output_unit=UnitFrequency.GIGAHERTZ,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
-    body: UnitIlluminanceConversion = result
+    body: UnitFrequencyConversion = result
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
-        Optional[Union[UnitIlluminanceConversion, Error]]
-    ] = get_illuminance_unit_conversion.sync_detailed(
+        Optional[Union[UnitFrequencyConversion, Error]]
+    ] = get_frequency_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitIlluminanceFormat.LUX,
-        src_format=UnitIlluminanceFormat.LUX,
+        input_unit=UnitFrequency.GIGAHERTZ,
+        output_unit=UnitFrequency.GIGAHERTZ,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
-async def test_get_illuminance_unit_conversion_async():
+async def test_get_frequency_unit_conversion_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitIlluminanceConversion, Error]
-    ] = await get_illuminance_unit_conversion.asyncio(
+        Union[UnitFrequencyConversion, Error]
+    ] = await get_frequency_unit_conversion.asyncio(
         client=client,
-        output_format=UnitIlluminanceFormat.LUX,
-        src_format=UnitIlluminanceFormat.LUX,
+        input_unit=UnitFrequency.GIGAHERTZ,
+        output_unit=UnitFrequency.GIGAHERTZ,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
-        Optional[Union[UnitIlluminanceConversion, Error]]
-    ] = await get_illuminance_unit_conversion.asyncio_detailed(
+        Optional[Union[UnitFrequencyConversion, Error]]
+    ] = await get_frequency_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitIlluminanceFormat.LUX,
-        src_format=UnitIlluminanceFormat.LUX,
+        input_unit=UnitFrequency.GIGAHERTZ,
+        output_unit=UnitFrequency.GIGAHERTZ,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_length_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitLengthConversion, Error]
     ] = get_length_unit_conversion.sync(
         client=client,
-        output_format=UnitLengthFormat.METER,
-        src_format=UnitLengthFormat.METER,
+        input_unit=UnitLength.CENTIMETRES,
+        output_unit=UnitLength.CENTIMETRES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2463,16 +2063,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitLengthConversion, Error]]
     ] = get_length_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitLengthFormat.METER,
-        src_format=UnitLengthFormat.METER,
+        input_unit=UnitLength.CENTIMETRES,
+        output_unit=UnitLength.CENTIMETRES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2480,157 +2080,39 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitLengthConversion, Error]
     ] = await get_length_unit_conversion.asyncio(
         client=client,
-        output_format=UnitLengthFormat.METER,
-        src_format=UnitLengthFormat.METER,
+        input_unit=UnitLength.CENTIMETRES,
+        output_unit=UnitLength.CENTIMETRES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitLengthConversion, Error]]
     ] = await get_length_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitLengthFormat.METER,
-        src_format=UnitLengthFormat.METER,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_magnetic_field_strength_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMagneticFieldStrengthConversion, Error]
-    ] = get_magnetic_field_strength_unit_conversion.sync(
-        client=client,
-        output_format=UnitMagneticFieldStrengthFormat.TESLA,
-        src_format=UnitMagneticFieldStrengthFormat.TESLA,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitMagneticFieldStrengthConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitMagneticFieldStrengthConversion, Error]]
-    ] = get_magnetic_field_strength_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitMagneticFieldStrengthFormat.TESLA,
-        src_format=UnitMagneticFieldStrengthFormat.TESLA,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_magnetic_field_strength_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMagneticFieldStrengthConversion, Error]
-    ] = await get_magnetic_field_strength_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitMagneticFieldStrengthFormat.TESLA,
-        src_format=UnitMagneticFieldStrengthFormat.TESLA,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitMagneticFieldStrengthConversion, Error]]
-    ] = await get_magnetic_field_strength_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitMagneticFieldStrengthFormat.TESLA,
-        src_format=UnitMagneticFieldStrengthFormat.TESLA,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_magnetic_flux_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMagneticFluxConversion, Error]
-    ] = get_magnetic_flux_unit_conversion.sync(
-        client=client,
-        output_format=UnitMagneticFluxFormat.WEBER,
-        src_format=UnitMagneticFluxFormat.WEBER,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitMagneticFluxConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitMagneticFluxConversion, Error]]
-    ] = get_magnetic_flux_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitMagneticFluxFormat.WEBER,
-        src_format=UnitMagneticFluxFormat.WEBER,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_magnetic_flux_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMagneticFluxConversion, Error]
-    ] = await get_magnetic_flux_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitMagneticFluxFormat.WEBER,
-        src_format=UnitMagneticFluxFormat.WEBER,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitMagneticFluxConversion, Error]]
-    ] = await get_magnetic_flux_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitMagneticFluxFormat.WEBER,
-        src_format=UnitMagneticFluxFormat.WEBER,
+        input_unit=UnitLength.CENTIMETRES,
+        output_unit=UnitLength.CENTIMETRES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_mass_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[UnitMassConversion, Error]] = get_mass_unit_conversion.sync(
         client=client,
-        output_format=UnitMassFormat.GRAM,
-        src_format=UnitMassFormat.GRAM,
+        input_unit=UnitMass.CARATS,
+        output_unit=UnitMass.CARATS,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2638,16 +2120,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitMassConversion, Error]]
     ] = get_mass_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitMassFormat.GRAM,
-        src_format=UnitMassFormat.GRAM,
+        input_unit=UnitMass.CARATS,
+        output_unit=UnitMass.CARATS,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2655,218 +2137,41 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitMassConversion, Error]
     ] = await get_mass_unit_conversion.asyncio(
         client=client,
-        output_format=UnitMassFormat.GRAM,
-        src_format=UnitMassFormat.GRAM,
+        input_unit=UnitMass.CARATS,
+        output_unit=UnitMass.CARATS,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitMassConversion, Error]]
     ] = await get_mass_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitMassFormat.GRAM,
-        src_format=UnitMassFormat.GRAM,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_metric_power_cubed_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerCubedConversion, Error]
-    ] = get_metric_power_cubed_unit_conversion.sync(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitMetricPowerCubedConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitMetricPowerCubedConversion, Error]]
-    ] = get_metric_power_cubed_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_metric_power_cubed_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerCubedConversion, Error]
-    ] = await get_metric_power_cubed_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitMetricPowerCubedConversion, Error]]
-    ] = await get_metric_power_cubed_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_metric_power_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerConversion, Error]
-    ] = get_metric_power_unit_conversion.sync(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitMetricPowerConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitMetricPowerConversion, Error]]
-    ] = get_metric_power_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_metric_power_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerConversion, Error]
-    ] = await get_metric_power_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitMetricPowerConversion, Error]]
-    ] = await get_metric_power_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_metric_power_squared_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerSquaredConversion, Error]
-    ] = get_metric_power_squared_unit_conversion.sync(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitMetricPowerSquaredConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitMetricPowerSquaredConversion, Error]]
-    ] = get_metric_power_squared_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_metric_power_squared_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitMetricPowerSquaredConversion, Error]
-    ] = await get_metric_power_squared_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitMetricPowerSquaredConversion, Error]]
-    ] = await get_metric_power_squared_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitMetricPower.ATTO,
-        src_format=UnitMetricPower.ATTO,
+        input_unit=UnitMass.CARATS,
+        output_unit=UnitMass.CARATS,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_power_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitPowerConversion, Error]
     ] = get_power_unit_conversion.sync(
         client=client,
-        output_format=UnitPowerFormat.WATT,
-        src_format=UnitPowerFormat.WATT,
+        input_unit=UnitPower.BTU_PER_MINUTE,
+        output_unit=UnitPower.BTU_PER_MINUTE,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2874,16 +2179,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitPowerConversion, Error]]
     ] = get_power_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitPowerFormat.WATT,
-        src_format=UnitPowerFormat.WATT,
+        input_unit=UnitPower.BTU_PER_MINUTE,
+        output_unit=UnitPower.BTU_PER_MINUTE,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2891,41 +2196,41 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitPowerConversion, Error]
     ] = await get_power_unit_conversion.asyncio(
         client=client,
-        output_format=UnitPowerFormat.WATT,
-        src_format=UnitPowerFormat.WATT,
+        input_unit=UnitPower.BTU_PER_MINUTE,
+        output_unit=UnitPower.BTU_PER_MINUTE,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitPowerConversion, Error]]
     ] = await get_power_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitPowerFormat.WATT,
-        src_format=UnitPowerFormat.WATT,
+        input_unit=UnitPower.BTU_PER_MINUTE,
+        output_unit=UnitPower.BTU_PER_MINUTE,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_pressure_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitPressureConversion, Error]
     ] = get_pressure_unit_conversion.sync(
         client=client,
-        output_format=UnitPressureFormat.PASCAL,
-        src_format=UnitPressureFormat.PASCAL,
+        input_unit=UnitPressure.ATMOSPHERES,
+        output_unit=UnitPressure.ATMOSPHERES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2933,16 +2238,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitPressureConversion, Error]]
     ] = get_pressure_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitPressureFormat.PASCAL,
-        src_format=UnitPressureFormat.PASCAL,
+        input_unit=UnitPressure.ATMOSPHERES,
+        output_unit=UnitPressure.ATMOSPHERES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2950,218 +2255,41 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitPressureConversion, Error]
     ] = await get_pressure_unit_conversion.asyncio(
         client=client,
-        output_format=UnitPressureFormat.PASCAL,
-        src_format=UnitPressureFormat.PASCAL,
+        input_unit=UnitPressure.ATMOSPHERES,
+        output_unit=UnitPressure.ATMOSPHERES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitPressureConversion, Error]]
     ] = await get_pressure_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitPressureFormat.PASCAL,
-        src_format=UnitPressureFormat.PASCAL,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_radiation_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitRadiationConversion, Error]
-    ] = get_radiation_unit_conversion.sync(
-        client=client,
-        output_format=UnitRadiationFormat.GRAY,
-        src_format=UnitRadiationFormat.GRAY,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitRadiationConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitRadiationConversion, Error]]
-    ] = get_radiation_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitRadiationFormat.GRAY,
-        src_format=UnitRadiationFormat.GRAY,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_radiation_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitRadiationConversion, Error]
-    ] = await get_radiation_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitRadiationFormat.GRAY,
-        src_format=UnitRadiationFormat.GRAY,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitRadiationConversion, Error]]
-    ] = await get_radiation_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitRadiationFormat.GRAY,
-        src_format=UnitRadiationFormat.GRAY,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_radioactivity_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitRadioactivityConversion, Error]
-    ] = get_radioactivity_unit_conversion.sync(
-        client=client,
-        output_format=UnitRadioactivityFormat.BECQUEREL,
-        src_format=UnitRadioactivityFormat.BECQUEREL,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitRadioactivityConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitRadioactivityConversion, Error]]
-    ] = get_radioactivity_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitRadioactivityFormat.BECQUEREL,
-        src_format=UnitRadioactivityFormat.BECQUEREL,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_radioactivity_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitRadioactivityConversion, Error]
-    ] = await get_radioactivity_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitRadioactivityFormat.BECQUEREL,
-        src_format=UnitRadioactivityFormat.BECQUEREL,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitRadioactivityConversion, Error]]
-    ] = await get_radioactivity_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitRadioactivityFormat.BECQUEREL,
-        src_format=UnitRadioactivityFormat.BECQUEREL,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_solid_angle_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitSolidAngleConversion, Error]
-    ] = get_solid_angle_unit_conversion.sync(
-        client=client,
-        output_format=UnitSolidAngleFormat.STERADIAN,
-        src_format=UnitSolidAngleFormat.STERADIAN,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitSolidAngleConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitSolidAngleConversion, Error]]
-    ] = get_solid_angle_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitSolidAngleFormat.STERADIAN,
-        src_format=UnitSolidAngleFormat.STERADIAN,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_solid_angle_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitSolidAngleConversion, Error]
-    ] = await get_solid_angle_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitSolidAngleFormat.STERADIAN,
-        src_format=UnitSolidAngleFormat.STERADIAN,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitSolidAngleConversion, Error]]
-    ] = await get_solid_angle_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitSolidAngleFormat.STERADIAN,
-        src_format=UnitSolidAngleFormat.STERADIAN,
+        input_unit=UnitPressure.ATMOSPHERES,
+        output_unit=UnitPressure.ATMOSPHERES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_temperature_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitTemperatureConversion, Error]
     ] = get_temperature_unit_conversion.sync(
         client=client,
-        output_format=UnitTemperatureFormat.KELVIN,
-        src_format=UnitTemperatureFormat.KELVIN,
+        input_unit=UnitTemperature.CELSIUS,
+        output_unit=UnitTemperature.CELSIUS,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -3169,16 +2297,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitTemperatureConversion, Error]]
     ] = get_temperature_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitTemperatureFormat.KELVIN,
-        src_format=UnitTemperatureFormat.KELVIN,
+        input_unit=UnitTemperature.CELSIUS,
+        output_unit=UnitTemperature.CELSIUS,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -3186,216 +2314,100 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitTemperatureConversion, Error]
     ] = await get_temperature_unit_conversion.asyncio(
         client=client,
-        output_format=UnitTemperatureFormat.KELVIN,
-        src_format=UnitTemperatureFormat.KELVIN,
+        input_unit=UnitTemperature.CELSIUS,
+        output_unit=UnitTemperature.CELSIUS,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitTemperatureConversion, Error]]
     ] = await get_temperature_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitTemperatureFormat.KELVIN,
-        src_format=UnitTemperatureFormat.KELVIN,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_time_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[Union[UnitTimeConversion, Error]] = get_time_unit_conversion.sync(
-        client=client,
-        output_format=UnitTimeFormat.SECOND,
-        src_format=UnitTimeFormat.SECOND,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitTimeConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitTimeConversion, Error]]
-    ] = get_time_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitTimeFormat.SECOND,
-        src_format=UnitTimeFormat.SECOND,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_time_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitTimeConversion, Error]
-    ] = await get_time_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitTimeFormat.SECOND,
-        src_format=UnitTimeFormat.SECOND,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitTimeConversion, Error]]
-    ] = await get_time_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitTimeFormat.SECOND,
-        src_format=UnitTimeFormat.SECOND,
-        value=3.14,
-    )
-
-
-@pytest.mark.skip
-def test_get_velocity_unit_conversion():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitVelocityConversion, Error]
-    ] = get_velocity_unit_conversion.sync(
-        client=client,
-        output_format=UnitVelocityFormat.METERS_PER_SECOND,
-        src_format=UnitVelocityFormat.METERS_PER_SECOND,
-        value=3.14,
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: UnitVelocityConversion = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[UnitVelocityConversion, Error]]
-    ] = get_velocity_unit_conversion.sync_detailed(
-        client=client,
-        output_format=UnitVelocityFormat.METERS_PER_SECOND,
-        src_format=UnitVelocityFormat.METERS_PER_SECOND,
-        value=3.14,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_velocity_unit_conversion_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[
-        Union[UnitVelocityConversion, Error]
-    ] = await get_velocity_unit_conversion.asyncio(
-        client=client,
-        output_format=UnitVelocityFormat.METERS_PER_SECOND,
-        src_format=UnitVelocityFormat.METERS_PER_SECOND,
-        value=3.14,
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[UnitVelocityConversion, Error]]
-    ] = await get_velocity_unit_conversion.asyncio_detailed(
-        client=client,
-        output_format=UnitVelocityFormat.METERS_PER_SECOND,
-        src_format=UnitVelocityFormat.METERS_PER_SECOND,
+        input_unit=UnitTemperature.CELSIUS,
+        output_unit=UnitTemperature.CELSIUS,
         value=3.14,
     )
 
 
 @pytest.mark.skip
-def test_get_voltage_unit_conversion():
+def test_get_torque_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitVoltageConversion, Error]
-    ] = get_voltage_unit_conversion.sync(
+        Union[UnitTorqueConversion, Error]
+    ] = get_torque_unit_conversion.sync(
         client=client,
-        output_format=UnitVoltageFormat.VOLT,
-        src_format=UnitVoltageFormat.VOLT,
+        input_unit=UnitTorque.NEWTON_METRES,
+        output_unit=UnitTorque.NEWTON_METRES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
-    body: UnitVoltageConversion = result
+    body: UnitTorqueConversion = result
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
-        Optional[Union[UnitVoltageConversion, Error]]
-    ] = get_voltage_unit_conversion.sync_detailed(
+        Optional[Union[UnitTorqueConversion, Error]]
+    ] = get_torque_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitVoltageFormat.VOLT,
-        src_format=UnitVoltageFormat.VOLT,
+        input_unit=UnitTorque.NEWTON_METRES,
+        output_unit=UnitTorque.NEWTON_METRES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
-async def test_get_voltage_unit_conversion_async():
+async def test_get_torque_unit_conversion_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
-        Union[UnitVoltageConversion, Error]
-    ] = await get_voltage_unit_conversion.asyncio(
+        Union[UnitTorqueConversion, Error]
+    ] = await get_torque_unit_conversion.asyncio(
         client=client,
-        output_format=UnitVoltageFormat.VOLT,
-        src_format=UnitVoltageFormat.VOLT,
+        input_unit=UnitTorque.NEWTON_METRES,
+        output_unit=UnitTorque.NEWTON_METRES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
-        Optional[Union[UnitVoltageConversion, Error]]
-    ] = await get_voltage_unit_conversion.asyncio_detailed(
+        Optional[Union[UnitTorqueConversion, Error]]
+    ] = await get_torque_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitVoltageFormat.VOLT,
-        src_format=UnitVoltageFormat.VOLT,
+        input_unit=UnitTorque.NEWTON_METRES,
+        output_unit=UnitTorque.NEWTON_METRES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_volume_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitVolumeConversion, Error]
     ] = get_volume_unit_conversion.sync(
         client=client,
-        output_format=UnitVolumeFormat.CUBIC_METER,
-        src_format=UnitVolumeFormat.CUBIC_METER,
+        input_unit=UnitVolume.CUBIC_CENTIMETRES,
+        output_unit=UnitVolume.CUBIC_CENTIMETRES,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -3403,16 +2415,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitVolumeConversion, Error]]
     ] = get_volume_unit_conversion.sync_detailed(
         client=client,
-        output_format=UnitVolumeFormat.CUBIC_METER,
-        src_format=UnitVolumeFormat.CUBIC_METER,
+        input_unit=UnitVolume.CUBIC_CENTIMETRES,
+        output_unit=UnitVolume.CUBIC_CENTIMETRES,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -3420,26 +2432,26 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitVolumeConversion, Error]
     ] = await get_volume_unit_conversion.asyncio(
         client=client,
-        output_format=UnitVolumeFormat.CUBIC_METER,
-        src_format=UnitVolumeFormat.CUBIC_METER,
+        input_unit=UnitVolume.CUBIC_CENTIMETRES,
+        output_unit=UnitVolume.CUBIC_CENTIMETRES,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitVolumeConversion, Error]]
     ] = await get_volume_unit_conversion.asyncio_detailed(
         client=client,
-        output_format=UnitVolumeFormat.CUBIC_METER,
-        src_format=UnitVolumeFormat.CUBIC_METER,
+        input_unit=UnitVolume.CUBIC_CENTIMETRES,
+        output_unit=UnitVolume.CUBIC_CENTIMETRES,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_delete_user_self():
     # Create our client.
```

### Comparing `kittycad-0.4.2/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.3/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.3/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.3/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_call_query_group.py` & `kittycad-0.4.3/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.3/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_call_status.py` & `kittycad-0.4.3/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_call_with_price.py` & `kittycad-0.4.3/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.3/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_token.py` & `kittycad-0.4.3/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/api_token_results_page.py` & `kittycad-0.4.3/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/app_client_info.py` & `kittycad-0.4.3/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/async_api_call.py` & `kittycad-0.4.3/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/async_api_call_output.py` & `kittycad-0.4.3/kittycad/models/async_api_call_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.3/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/async_api_call_type.py` & `kittycad-0.4.3/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/billing_info.py` & `kittycad-0.4.3/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/cache_metadata.py` & `kittycad-0.4.3/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/card_details.py` & `kittycad-0.4.3/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/cluster.py` & `kittycad-0.4.3/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/code_output.py` & `kittycad-0.4.3/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/commit.py` & `kittycad-0.4.3/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/connection.py` & `kittycad-0.4.3/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/country_code.py` & `kittycad-0.4.3/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/currency.py` & `kittycad-0.4.3/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/customer.py` & `kittycad-0.4.3/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/customer_balance.py` & `kittycad-0.4.3/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.3/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.3/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.3/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/docker_system_info.py` & `kittycad-0.4.3/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/email_authentication_form.py` & `kittycad-0.4.3/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/engine_metadata.py` & `kittycad-0.4.3/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/environment.py` & `kittycad-0.4.3/kittycad/models/environment.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/error.py` & `kittycad-0.4.3/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/executor_metadata.py` & `kittycad-0.4.3/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/extended_user.py` & `kittycad-0.4.3/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.3/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/extrude.py` & `kittycad-0.4.3/kittycad/models/extrude.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.3/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_conversion.py` & `kittycad-0.4.3/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_density.py` & `kittycad-0.4.3/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_export_format.py` & `kittycad-0.4.3/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_import_format.py` & `kittycad-0.4.3/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_mass.py` & `kittycad-0.4.3/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_surface_area.py` & `kittycad-0.4.3/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_system_metadata.py` & `kittycad-0.4.3/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/file_volume.py` & `kittycad-0.4.3/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/gateway.py` & `kittycad-0.4.3/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/index_info.py` & `kittycad-0.4.3/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/invoice.py` & `kittycad-0.4.3/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/invoice_line_item.py` & `kittycad-0.4.3/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/invoice_status.py` & `kittycad-0.4.3/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/jetstream.py` & `kittycad-0.4.3/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.3/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/jetstream_config.py` & `kittycad-0.4.3/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/jetstream_stats.py` & `kittycad-0.4.3/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/leaf_node.py` & `kittycad-0.4.3/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/line3d.py` & `kittycad-0.4.3/kittycad/models/line3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/mesh.py` & `kittycad-0.4.3/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.3/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/metadata.py` & `kittycad-0.4.3/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/method.py` & `kittycad-0.4.3/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_cmd.py` & `kittycad-0.4.3/kittycad/models/modeling_cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_cmd_req.py` & `kittycad-0.4.3/kittycad/models/modeling_cmd_req.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_cmd_req_batch.py` & `kittycad-0.4.3/kittycad/models/modeling_cmd_req_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_error.py` & `kittycad-0.4.3/kittycad/models/modeling_error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_outcome.py` & `kittycad-0.4.3/kittycad/models/modeling_outcome.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/modeling_outcomes.py` & `kittycad-0.4.3/kittycad/models/modeling_outcomes.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/new_address.py` & `kittycad-0.4.3/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.3/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/onboarding.py` & `kittycad-0.4.3/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/output_file.py` & `kittycad-0.4.3/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/payment_intent.py` & `kittycad-0.4.3/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/payment_method.py` & `kittycad-0.4.3/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.3/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/physics_constant.py` & `kittycad-0.4.3/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/physics_constant_name.py` & `kittycad-0.4.3/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/plugins_info.py` & `kittycad-0.4.3/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/point2d.py` & `kittycad-0.4.3/kittycad/models/point2d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/point3d.py` & `kittycad-0.4.3/kittycad/models/point3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/point_e_metadata.py` & `kittycad-0.4.3/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/pong.py` & `kittycad-0.4.3/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/registry_service_config.py` & `kittycad-0.4.3/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/runtime.py` & `kittycad-0.4.3/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/session.py` & `kittycad-0.4.3/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.3/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_temperature_conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_acceleration_format import UnitAccelerationFormat
+from ..models.unit_temperature import UnitTemperature
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitAccelerationConversion")
+E = TypeVar("E", bound="UnitTemperatureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAccelerationConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitTemperatureConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitTemperature] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAccelerationFormat] = UNSET
-    src_format: Union[Unset, UnitAccelerationFormat] = UNSET
+    output_unit: Union[Unset, UnitTemperature] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitTemperature]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitTemperature(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAccelerationFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitAccelerationFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAccelerationFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitTemperature]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitAccelerationFormat(_src_format)
+            output_unit = UnitTemperature(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_acceleration_conversion = cls(
+        unit_temperature_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_acceleration_conversion.additional_properties = d
-        return unit_acceleration_conversion
+        unit_temperature_conversion.additional_properties = d
+        return unit_temperature_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_volume_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_angle_format import UnitAngleFormat
+from ..models.unit_volume import UnitVolume
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="UnitAngleConversion")
+Q = TypeVar("Q", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAngleConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitVolumeConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitVolume] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAngleFormat] = UNSET
-    src_format: Union[Unset, UnitAngleFormat] = UNSET
+    output_unit: Union[Unset, UnitVolume] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitVolume]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitVolume(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAngleFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitAngleFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAngleFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitVolume]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitAngleFormat(_src_format)
+            output_unit = UnitVolume(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_angle_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_angle_conversion.additional_properties = d
-        return unit_angle_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_angle_format.py` & `kittycad-0.4.3/kittycad/models/unit_power.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from enum import Enum
 
 
-class UnitAngleFormat(str, Enum):
-    """The valid types of angle formats."""  # noqa: E501
+class UnitPower(str, Enum):
+    """The valid types of power units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Radian> """  # noqa: E501
-    RADIAN = "radian"
-    """# <https://en.wikipedia.org/wiki/Degree_(angle)> """  # noqa: E501
-    DEGREE = "degree"
-    """# <https://en.wikipedia.org/wiki/Minute_and_second_of_arc> """  # noqa: E501
-    ARCMINUTE = "arcminute"
-    """# <https://en.wikipedia.org/wiki/Minute_and_second_of_arc> """  # noqa: E501
-    ARCSECOND = "arcsecond"
-    """# <https://en.wikipedia.org/wiki/Minute_and_second_of_arc#Symbols_and_abbreviations> """  # noqa: E501
-    MILLIARCSECOND = "milliarcsecond"
-    """# <https://en.wikipedia.org/wiki/Turn_(angle)> """  # noqa: E501
-    TURN = "turn"
-    """# <https://en.wikipedia.org/wiki/Gradian> """  # noqa: E501
-    GRADIAN = "gradian"
+    """# British thermal units (BTU) per minute <https://en.wikipedia.org/wiki/British_thermal_unit> """  # noqa: E501
+    BTU_PER_MINUTE = "btu_per_minute"
+    """# Horsepower (hp) <https://en.wikipedia.org/wiki/Horsepower> """  # noqa: E501
+    HORSEPOWER = "horsepower"
+    """# Kilowatts <https://en.wikipedia.org/wiki/Kilowatt> """  # noqa: E501
+    KILOWATTS = "kilowatts"
+    """# Metric horsepower (PS) <https://en.wikipedia.org/wiki/Horsepower#Metric_horsepower> """  # noqa: E501
+    METRIC_HORSEPOWER = "metric_horsepower"
+    """# Microwatts <https://en.wikipedia.org/wiki/Microwatt> """  # noqa: E501
+    MICROWATTS = "microwatts"
+    """# Millwatts <https://en.wikipedia.org/wiki/Milliwatt> """  # noqa: E501
+    MILLIWATTS = "milliwatts"
+    """# Watts <https://en.wikipedia.org/wiki/Watt> """  # noqa: E501
+    WATTS = "watts"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_mass_conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_angular_velocity_format import UnitAngularVelocityFormat
+from ..models.unit_mass import UnitMass
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitAngularVelocityConversion")
+N = TypeVar("N", bound="UnitMassConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAngularVelocityConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitMassConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitMass] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAngularVelocityFormat] = UNSET
-    src_format: Union[Unset, UnitAngularVelocityFormat] = UNSET
+    output_unit: Union[Unset, UnitMass] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitMass]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitMass(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAngularVelocityFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitAngularVelocityFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAngularVelocityFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitMass]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitAngularVelocityFormat(_src_format)
+            output_unit = UnitMass(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_angular_velocity_conversion = cls(
+        unit_mass_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_angular_velocity_conversion.additional_properties = d
-        return unit_angular_velocity_conversion
+        unit_mass_conversion.additional_properties = d
+        return unit_mass_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_angular_velocity_format.py` & `kittycad-0.4.3/kittycad/models/unit_energy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from enum import Enum
 
 
-class UnitAngularVelocityFormat(str, Enum):
-    """The valid types of angular velocity unit formats."""  # noqa: E501
+class UnitEnergy(str, Enum):
+    """The valid types of energy units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Radian_per_second> """  # noqa: E501
-    RADIANS_PER_SECOND = "radians_per_second"
-    """# <https://en.wikipedia.org/wiki/Rotational_speed> """  # noqa: E501
-    DEGREES_PER_SECOND = "degrees_per_second"
-    """# <https://en.wikipedia.org/wiki/Revolutions_per_minute> """  # noqa: E501
-    REVOLUTIONS_PER_MINUTE = "revolutions_per_minute"
-    """# <https://en.wikipedia.org/wiki/Minute_and_second_of_arc#Symbols_and_abbreviations> """  # noqa: E501
-    MILLIARCSECONDS_PER_YEAR = "milliarcseconds_per_year"
+    """# British Thermal Unit (BTU) <https://en.wikipedia.org/wiki/British_thermal_unit> """  # noqa: E501
+    BTU = "btu"
+    """# Electron Volts (eV) <https://en.wikipedia.org/wiki/Electronvolt> """  # noqa: E501
+    ELECTRONVOLTS = "electronvolts"
+    """# Joules (or watt-seconds) <https://en.wikipedia.org/wiki/Joule> """  # noqa: E501
+    JOULES = "joules"
+    """# Kilocalories (often just called calories) <https://en.wikipedia.org/wiki/Kilocalorie> """  # noqa: E501
+    KILOCALORIES = "kilocalories"
+    """# Kilowatt hours (kWh) <https://en.wikipedia.org/wiki/Kilowatt-hour> """  # noqa: E501
+    KILOWATT_HOURS = "kilowatt_hours"
+    """# Watt hours (Wh) <https://en.wikipedia.org/wiki/Kilowatt-hour> """  # noqa: E501
+    WATT_HOURS = "watt_hours"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_area_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_area_format import UnitAreaFormat
+from ..models.unit_area import UnitArea
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Z = TypeVar("Z", bound="UnitAreaConversion")
+D = TypeVar("D", bound="UnitAreaConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAreaConversion:
-    """A unit conversion."""  # noqa: E501
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitArea] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAreaFormat] = UNSET
-    src_format: Union[Unset, UnitAreaFormat] = UNSET
+    output_unit: Union[Unset, UnitArea] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitArea]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitArea(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAreaFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitAreaFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAreaFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitArea]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitAreaFormat(_src_format)
+            output_unit = UnitArea(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -155,17 +155,17 @@
 
         unit_area_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
         unit_area_conversion.additional_properties = d
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_area_format.py` & `kittycad-0.4.3/kittycad/models/unit_pressure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from enum import Enum
 
 
-class UnitAreaFormat(str, Enum):
-    """The valid types of area unit formats."""  # noqa: E501
+class UnitPressure(str, Enum):
+    """The valid types of pressure units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Square_metre> """  # noqa: E501
-    SQUARE_METER = "square_meter"
-    """# <https://en.wikipedia.org/wiki/Square_foot> """  # noqa: E501
-    SQUARE_FOOT = "square_foot"
-    """# <https://en.wikipedia.org/wiki/Square_inch> """  # noqa: E501
-    SQUARE_INCH = "square_inch"
-    """# <https://en.wikipedia.org/wiki/Square_mile> """  # noqa: E501
-    SQUARE_MILE = "square_mile"
-    """# <https://en.wikipedia.org/wiki/Square_kilometre> """  # noqa: E501
-    SQUARE_KILOMETER = "square_kilometer"
-    """# <https://en.wikipedia.org/wiki/Hectare> """  # noqa: E501
-    HECTARE = "hectare"
-    """# <https://en.wikipedia.org/wiki/Acre> """  # noqa: E501
-    ACRE = "acre"
+    """# Atmospheres <https://en.wikipedia.org/wiki/Standard_atmosphere_(unit)> """  # noqa: E501
+    ATMOSPHERES = "atmospheres"
+    """# Bars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
+    BARS = "bars"
+    """# Hectopascals <https://en.wikipedia.org/wiki/Hectopascal> """  # noqa: E501
+    HECTOPASCALS = "hectopascals"
+    """# Kilopascals <https://en.wikipedia.org/wiki/Kilopascal> """  # noqa: E501
+    KILOPASCALS = "kilopascals"
+    """# Millibars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
+    MILLIBARS = "millibars"
+    """# Pascals <https://en.wikipedia.org/wiki/Pascal_(unit)> """  # noqa: E501
+    PASCALS = "pascals"
+    """# Pounds per square inch (PSI) - <https://en.wikipedia.org/wiki/Pound_per_square_inch> """  # noqa: E501
+    PSI = "psi"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_charge_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_torque_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_charge_format import UnitChargeFormat
+from ..models.unit_torque import UnitTorque
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="UnitChargeConversion")
+T = TypeVar("T", bound="UnitTorqueConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitChargeConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitTorqueConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitTorque] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitChargeFormat] = UNSET
-    src_format: Union[Unset, UnitChargeFormat] = UNSET
+    output_unit: Union[Unset, UnitTorque] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitTorque]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitTorque(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitChargeFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitChargeFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitChargeFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitTorque]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitChargeFormat(_src_format)
+            output_unit = UnitTorque(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_charge_conversion = cls(
+        unit_torque_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_charge_conversion.additional_properties = d
-        return unit_charge_conversion
+        unit_torque_conversion.additional_properties = d
+        return unit_torque_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_current_conversion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_concentration_format import UnitConcentrationFormat
+from ..models.unit_current import UnitCurrent
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="UnitConcentrationConversion")
+F = TypeVar("F", bound="UnitCurrentConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitConcentrationConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitCurrentConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitCurrent] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitConcentrationFormat] = UNSET
-    src_format: Union[Unset, UnitConcentrationFormat] = UNSET
+    output_unit: Union[Unset, UnitCurrent] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitCurrent]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitCurrent(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitConcentrationFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitConcentrationFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitConcentrationFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitCurrent]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitConcentrationFormat(_src_format)
+            output_unit = UnitCurrent(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_concentration_conversion = cls(
+        unit_current_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_concentration_conversion.additional_properties = d
-        return unit_concentration_conversion
+        unit_current_conversion.additional_properties = d
+        return unit_current_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_concentration_format.py` & `kittycad-0.4.3/kittycad/models/unit_force.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from enum import Enum
 
 
-class UnitConcentrationFormat(str, Enum):
-    """The valid types of concentration unit formats."""  # noqa: E501
+class UnitForce(str, Enum):
+    """The valid types of force units."""  # noqa: E501
 
-    """# Per Million - <https://en.wikipedia.org/wiki/Parts-per_notation> """  # noqa: E501
-    PARTS_PER_MILLION = "parts_per_million"
-    """# Per Billion - <https://en.wikipedia.org/wiki/Parts-per_notation> """  # noqa: E501
-    PARTS_PER_BILLION = "parts_per_billion"
-    """# Per Trillion - <https://en.wikipedia.org/wiki/Parts-per_notation> """  # noqa: E501
-    PARTS_PER_TRILLION = "parts_per_trillion"
-    """# <https://en.wikipedia.org/wiki/Concentration>, <https://en.wikipedia.org/wiki/Percentage> """  # noqa: E501
-    PERCENT = "percent"
+    """# Dynes <https://en.wikipedia.org/wiki/Dyne> """  # noqa: E501
+    DYNES = "dynes"
+    """# Kiloponds <https://en.wikipedia.org/wiki/Kilopond> """  # noqa: E501
+    KILOPONDS = "kiloponds"
+    """# Micronewtons <https://en.wikipedia.org/wiki/Newton_(unit)> """  # noqa: E501
+    MICRONEWTONS = "micronewtons"
+    """# Millinewtons <https://en.wikipedia.org/wiki/Newton_(unit)> """  # noqa: E501
+    MILLINEWTONS = "millinewtons"
+    """# Newtons <https://en.wikipedia.org/wiki/Newton_(unit)> """  # noqa: E501
+    NEWTONS = "newtons"
+    """# Poundals <https://en.wikipedia.org/wiki/Poundal> """  # noqa: E501
+    POUNDALS = "poundals"
+    """# Pounds <https://en.wikipedia.org/wiki/Pound_(force)> """  # noqa: E501
+    POUNDS = "pounds"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_data_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_angle_conversion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_data_format import UnitDataFormat
+from ..models.unit_angle import UnitAngle
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitDataConversion")
+Y = TypeVar("Y", bound="UnitAngleConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitDataConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitAngleConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitAngle] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitDataFormat] = UNSET
-    src_format: Union[Unset, UnitDataFormat] = UNSET
+    output_unit: Union[Unset, UnitAngle] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitAngle]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitAngle(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitDataFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitDataFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitDataFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitAngle]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitDataFormat(_src_format)
+            output_unit = UnitAngle(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_data_conversion = cls(
+        unit_angle_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_data_conversion.additional_properties = d
-        return unit_data_conversion
+        unit_angle_conversion.additional_properties = d
+        return unit_angle_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_length_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
+from ..models.unit_length import UnitLength
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitDataTransferRateConversion")
+N = TypeVar("N", bound="UnitLengthConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitDataTransferRateConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitLengthConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitLength] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitDataTransferRateFormat] = UNSET
-    src_format: Union[Unset, UnitDataTransferRateFormat] = UNSET
+    output_unit: Union[Unset, UnitLength] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,20 +65,20 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitLength]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitLength(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitDataTransferRateFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitDataTransferRateFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitDataTransferRateFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitLength]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitDataTransferRateFormat(_src_format)
+            output_unit = UnitLength(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_data_transfer_rate_conversion = cls(
+        unit_length_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_data_transfer_rate_conversion.additional_properties = d
-        return unit_data_transfer_rate_conversion
+        unit_length_conversion.additional_properties = d
+        return unit_length_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_density_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_pressure_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_density_format import UnitDensityFormat
+from ..models.unit_pressure import UnitPressure
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="UnitDensityConversion")
+V = TypeVar("V", bound="UnitPressureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitDensityConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitPressureConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitPressure] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitDensityFormat] = UNSET
-    src_format: Union[Unset, UnitDensityFormat] = UNSET
+    output_unit: Union[Unset, UnitPressure] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitPressure]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitPressure(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitDensityFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitDensityFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitDensityFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitPressure]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitDensityFormat(_src_format)
+            output_unit = UnitPressure(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_density_conversion = cls(
+        unit_pressure_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_density_conversion.additional_properties = d
-        return unit_density_conversion
+        unit_pressure_conversion.additional_properties = d
+        return unit_pressure_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_density_format.py` & `kittycad-0.4.3/kittycad/models/unit_mass.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 from enum import Enum
 
 
-class UnitDensityFormat(str, Enum):
-    """The valid types of density unit formats."""  # noqa: E501
+class UnitMass(str, Enum):
+    """The valid types of mass units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Kilogram_per_cubic_metre> """  # noqa: E501
-    KILOGRAMS_PER_CUBIC_METER = "kilograms_per_cubic_meter"
-    """# <https://en.wikipedia.org/wiki/Specific_density> """  # noqa: E501
-    GRAMS_PER_MILLILITER = "grams_per_milliliter"
-    """# <https://en.wikipedia.org/wiki/Kilogram_per_cubic_metre> """  # noqa: E501
-    KILOGRAMS_PER_LITER = "kilograms_per_liter"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    OUNCES_PER_CUBIC_FOOT = "ounces_per_cubic_foot"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    OUNCES_PER_CUBIC_INCH = "ounces_per_cubic_inch"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    OUNCES_PER_GALLON = "ounces_per_gallon"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    POUNDS_PER_CUBIC_FOOT = "pounds_per_cubic_foot"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    POUNDS_PER_CUBIC_INCH = "pounds_per_cubic_inch"
-    """# <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    POUNDS_PER_GALLON = "pounds_per_gallon"
-    """# <https://en.wikipedia.org/wiki/Slug_(unit)> and <https://en.wikipedia.org/wiki/Density#Unit> """  # noqa: E501
-    SLUGS_PER_CUBIC_FOOT = "slugs_per_cubic_foot"
+    """# Carats <https://en.wikipedia.org/wiki/Carat_(mass)> """  # noqa: E501
+    CARATS = "carats"
+    """# Grains <https://en.wikipedia.org/wiki/Grain_(unit)> """  # noqa: E501
+    GRAINS = "grains"
+    """# Grams <https://en.wikipedia.org/wiki/Gram> """  # noqa: E501
+    GRAMS = "grams"
+    """# Kilograms <https://en.wikipedia.org/wiki/Kilogram> """  # noqa: E501
+    KILOGRAMS = "kilograms"
+    """# Long tons <https://en.wikipedia.org/wiki/Long_ton> """  # noqa: E501
+    LONG_TONS = "long_tons"
+    """# Metric tons <https://en.wikipedia.org/wiki/Tonne> """  # noqa: E501
+    METRIC_TONS = "metric_tons"
+    """# Micrograms <https://en.wikipedia.org/wiki/Microgram> """  # noqa: E501
+    MICROGRAMS = "micrograms"
+    """# Milligrams <https://en.wikipedia.org/wiki/Milligram> """  # noqa: E501
+    MILLIGRAMS = "milligrams"
+    """# Ounces <https://en.wikipedia.org/wiki/Ounce> """  # noqa: E501
+    OUNCES = "ounces"
+    """# Pennyweights <https://en.wikipedia.org/wiki/Pennyweight> """  # noqa: E501
+    PENNYWEIGHTS = "pennyweights"
+    """# Pounds <https://en.wikipedia.org/wiki/Pound_(mass)> """  # noqa: E501
+    POUNDS = "pounds"
+    """# Short tons <https://en.wikipedia.org/wiki/Short_ton> """  # noqa: E501
+    SHORT_TONS = "short_tons"
+    """# Stones <https://en.wikipedia.org/wiki/Stone_(unit)> """  # noqa: E501
+    STONES = "stones"
+    """# Troy ounces <https://en.wikipedia.org/wiki/Troy_ounce> """  # noqa: E501
+    TROY_OUNCES = "troy_ounces"
+    """# Troy pounds <https://en.wikipedia.org/wiki/Troy_pound> """  # noqa: E501
+    TROY_POUNDS = "troy_pounds"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_force_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_energy_format import UnitEnergyFormat
+from ..models.unit_force import UnitForce
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="UnitEnergyConversion")
+G = TypeVar("G", bound="UnitForceConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitEnergyConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitForceConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitForce] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitEnergyFormat] = UNSET
-    src_format: Union[Unset, UnitEnergyFormat] = UNSET
+    output_unit: Union[Unset, UnitForce] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitForce]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitForce(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitEnergyFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitEnergyFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitEnergyFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitForce]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitEnergyFormat(_src_format)
+            output_unit = UnitForce(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_energy_conversion = cls(
+        unit_force_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_energy_conversion.additional_properties = d
-        return unit_energy_conversion
+        unit_force_conversion.additional_properties = d
+        return unit_force_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_power_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_force_format import UnitForceFormat
+from ..models.unit_power import UnitPower
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="UnitForceConversion")
+H = TypeVar("H", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitForceConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitPowerConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitPower] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitForceFormat] = UNSET
-    src_format: Union[Unset, UnitForceFormat] = UNSET
+    output_unit: Union[Unset, UnitPower] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitPower]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitPower(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitForceFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitForceFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitForceFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitPower]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitForceFormat(_src_format)
+            output_unit = UnitPower(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_force_conversion = cls(
+        unit_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_force_conversion.additional_properties = d
-        return unit_force_conversion
+        unit_power_conversion.additional_properties = d
+        return unit_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_frequency_conversion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_illuminance_format import UnitIlluminanceFormat
+from ..models.unit_frequency import UnitFrequency
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitIlluminanceConversion")
+L = TypeVar("L", bound="UnitFrequencyConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitIlluminanceConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitFrequencyConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitFrequency] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitIlluminanceFormat] = UNSET
-    src_format: Union[Unset, UnitIlluminanceFormat] = UNSET
+    output_unit: Union[Unset, UnitFrequency] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitFrequency]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitFrequency(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitIlluminanceFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitIlluminanceFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitIlluminanceFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitFrequency]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitIlluminanceFormat(_src_format)
+            output_unit = UnitFrequency(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_illuminance_conversion = cls(
+        unit_frequency_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_illuminance_conversion.additional_properties = d
-        return unit_illuminance_conversion
+        unit_frequency_conversion.additional_properties = d
+        return unit_frequency_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_illuminance_format.py` & `kittycad-0.4.3/kittycad/models/unit_temperature.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 
 
-class UnitIlluminanceFormat(str, Enum):
-    """The valid types of illuminance unit formats."""  # noqa: E501
+class UnitTemperature(str, Enum):
+    """The valid types of temperature units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Lux> """  # noqa: E501
-    LUX = "lux"
-    """# <https://en.wikipedia.org/wiki/Foot-candle> """  # noqa: E501
-    FOOTCANDLE = "footcandle"
-    """# <https://en.wikipedia.org/wiki/Lumen_(unit)> """  # noqa: E501
-    LUMENS_PER_SQUARE_INCH = "lumens_per_square_inch"
-    """# <https://en.wikipedia.org/wiki/Phot> """  # noqa: E501
-    PHOT = "phot"
+    """# Celsius <https://en.wikipedia.org/wiki/Celsius> """  # noqa: E501
+    CELSIUS = "celsius"
+    """# Fahrenheit <https://en.wikipedia.org/wiki/Fahrenheit> """  # noqa: E501
+    FAHRENHEIT = "fahrenheit"
+    """# Kelvin <https://en.wikipedia.org/wiki/Kelvin> """  # noqa: E501
+    KELVIN = "kelvin"
+    """# Rankine <https://en.wikipedia.org/wiki/Rankine_scale> """  # noqa: E501
+    RANKINE = "rankine"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.3/kittycad/models/unit_energy_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_length_format import UnitLengthFormat
+from ..models.unit_energy import UnitEnergy
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="UnitLengthConversion")
+Z = TypeVar("Z", bound="UnitEnergyConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitLengthConversion:
-    """A unit conversion."""  # noqa: E501
+class UnitEnergyConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitEnergy] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitLengthFormat] = UNSET
-    src_format: Union[Unset, UnitLengthFormat] = UNSET
+    output_unit: Union[Unset, UnitEnergy] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,19 +37,19 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -65,33 +65,33 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if input is not UNSET:
             field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,29 +110,29 @@
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitEnergy]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = UnitEnergy(_input_unit)
+
         output = d.pop("output", UNSET)
 
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitLengthFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = UnitLengthFormat(_output_format)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitLengthFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitEnergy]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = UnitLengthFormat(_src_format)
+            output_unit = UnitEnergy(_output_unit)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_length_conversion = cls(
+        unit_energy_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
+            input_unit=input_unit,
             output=output,
-            output_format=output_format,
-            src_format=src_format,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_length_conversion.additional_properties = d
-        return unit_length_conversion
+        unit_energy_conversion.additional_properties = d
+        return unit_energy_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_length_format.py` & `kittycad-0.4.3/kittycad/models/unit_volume.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 from enum import Enum
 
 
-class UnitLengthFormat(str, Enum):
-    """The valid types of length unit formats."""  # noqa: E501
+class UnitVolume(str, Enum):
+    """The valid types of volume units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Metre> """  # noqa: E501
-    METER = "meter"
-    """# <https://en.wikipedia.org/wiki/Millimetre> """  # noqa: E501
-    MILLIMETER = "millimeter"
-    """# <https://en.wikipedia.org/wiki/Centimetre> """  # noqa: E501
-    CENTIMETER = "centimeter"
-    """# <https://en.wikipedia.org/wiki/Kilometre> """  # noqa: E501
-    KILOMETER = "kilometer"
-    """# <https://en.wikipedia.org/wiki/Foot_(unit)> """  # noqa: E501
-    FOOT = "foot"
-    """# <https://en.wikipedia.org/wiki/Thousandth_of_an_inch> """  # noqa: E501
-    MIL = "mil"
-    """# <https://en.wikipedia.org/wiki/Inch> """  # noqa: E501
-    INCH = "inch"
-    """# <https://en.wikipedia.org/wiki/Mile> """  # noqa: E501
-    MILE = "mile"
-    """# <https://en.wikipedia.org/wiki/Nautical_mile> """  # noqa: E501
-    NAUTICAL_MILE = "nautical_mile"
-    """# <https://en.wikipedia.org/wiki/Astronomical_unit> """  # noqa: E501
-    ASTRONOMICAL_UNIT = "astronomical_unit"
-    """# <https://en.wikipedia.org/wiki/Light-year> """  # noqa: E501
-    LIGHTYEAR = "lightyear"
-    """# <https://en.wikipedia.org/wiki/Parsec> """  # noqa: E501
-    PARSEC = "parsec"
-    """# <https://en.wikipedia.org/wiki/Angstrom> """  # noqa: E501
-    ANGSTROM = "angstrom"
-    """# <https://en.wikipedia.org/wiki/Cubit> """  # noqa: E501
-    CUBIT = "cubit"
-    """# <https://en.wikipedia.org/wiki/Fathom> """  # noqa: E501
-    FATHOM = "fathom"
-    """# <https://en.wikipedia.org/wiki/Chain_(unit)> """  # noqa: E501
-    CHAIN = "chain"
-    """# <https://en.wikipedia.org/wiki/Furlong> """  # noqa: E501
-    FURLONG = "furlong"
-    """# <https://en.wikipedia.org/wiki/Hand_(unit)> """  # noqa: E501
-    HAND = "hand"
-    """# <https://en.wikipedia.org/wiki/League_(unit)> """  # noqa: E501
-    LEAGUE = "league"
-    """# <https://en.wikipedia.org/wiki/List_of_nautical_units_of_measurement> """  # noqa: E501
-    NAUTICAL_LEAGUE = "nautical_league"
-    """# <https://en.wikipedia.org/wiki/Yard> """  # noqa: E501
-    YARD = "yard"
+    """# Cubic centimeters (cc or cm³) <https://en.wikipedia.org/wiki/Cubic_centimetre> """  # noqa: E501
+    CUBIC_CENTIMETRES = "cubic_centimetres"
+    """# Cubic feet (ft³) <https://en.wikipedia.org/wiki/Cubic_foot> """  # noqa: E501
+    CUBIC_FEET = "cubic_feet"
+    """# Cubic inches (cu in or in³) <https://en.wikipedia.org/wiki/Cubic_inch> """  # noqa: E501
+    CUBIC_INCHES = "cubic_inches"
+    """# Cubic metres (m³) <https://en.wikipedia.org/wiki/Cubic_metre> """  # noqa: E501
+    CUBIC_METRES = "cubic_metres"
+    """# Cubic yards (yd³) <https://en.wikipedia.org/wiki/Cubic_yard> """  # noqa: E501
+    CUBIC_YARDS = "cubic_yards"
+    """# Cups <https://en.wikipedia.org/wiki/Cup_(unit)> """  # noqa: E501
+    CUPS = "cups"
+    """# Drams <https://en.wikipedia.org/wiki/Fluid_dram> """  # noqa: E501
+    DRAMS = "drams"
+    """# Drops <https://en.wikipedia.org/wiki/Minim_(unit)> """  # noqa: E501
+    DROPS = "drops"
+    """# US Fluid Ounces (fl oz) <https://en.wikipedia.org/wiki/Fluid_ounce> """  # noqa: E501
+    FLUID_OUNCES = "fluid_ounces"
+    """# UK Fluid Ounces (fl oz) <https://en.wikipedia.org/wiki/Fluid_ounce> """  # noqa: E501
+    FLUID_OUNCES_UK = "fluid_ounces_uk"
+    """# US Gallons (gal US) <https://en.wikipedia.org/wiki/Gallon> """  # noqa: E501
+    GALLONS = "gallons"
+    """# UK/Imperial Gallons (gal) <https://en.wikipedia.org/wiki/Gallon> """  # noqa: E501
+    GALLONS_UK = "gallons_uk"
+    """# Liters (l) <https://en.wikipedia.org/wiki/Litre> """  # noqa: E501
+    LITRES = "litres"
+    """# Milliliters (ml) <https://en.wikipedia.org/wiki/Litre> """  # noqa: E501
+    MILLILITRES = "millilitres"
+    """# Pints <https://en.wikipedia.org/wiki/Pint> """  # noqa: E501
+    PINTS = "pints"
+    """# Pints in the United Kingdom (UK) <https://en.wikipedia.org/wiki/Pint> """  # noqa: E501
+    PINTS_UK = "pints_uk"
+    """# Quarts <https://en.wikipedia.org/wiki/Quart> """  # noqa: E501
+    QUARTS = "quarts"
+    """# Tablespoons (tbsp) <https://en.wikipedia.org/wiki/Tablespoon> """  # noqa: E501
+    TABLESPOONS = "tablespoons"
+    """# Teaspoons (tsp) <https://en.wikipedia.org/wiki/Teaspoon> """  # noqa: E501
+    TEASPOONS = "teaspoons"
 
     def __str__(self) -> str:
         return str(self.value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kittycad-0.4.2/kittycad/models/unit_radioactivity_format.py` & `kittycad-0.4.3/kittycad/models/unit_current.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from enum import Enum
 
 
-class UnitRadioactivityFormat(str, Enum):
-    """The valid types of radioactivity unit formats. These describe the amount of radiation emitted by a radioactive material."""  # noqa: E501
+class UnitCurrent(str, Enum):
+    """The valid types of current units."""  # noqa: E501
 
-    """# <https://en.wikipedia.org/wiki/Becquerel> """  # noqa: E501
-    BECQUEREL = "becquerel"
-    """# <https://en.wikipedia.org/wiki/Curie_(unit)> """  # noqa: E501
-    CURIE = "curie"
-    """# <https://en.wikipedia.org/wiki/Rutherford_(unit)> """  # noqa: E501
-    RUTHERFORD = "rutherford"
+    """# Amperes <https://en.wikipedia.org/wiki/Ampere> """  # noqa: E501
+    AMPERES = "amperes"
+    """# Microamperes <https://en.wikipedia.org/wiki/Microampere> """  # noqa: E501
+    MICROAMPERES = "microamperes"
+    """# Milliamperes <https://en.wikipedia.org/wiki/Milliampere> """  # noqa: E501
+    MILLIAMPERES = "milliamperes"
+    """# Nanoamperes <https://en.wikipedia.org/wiki/Nanoampere> """  # noqa: E501
+    NANOAMPERES = "nanoamperes"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.2/kittycad/models/update_user.py` & `kittycad-0.4.3/kittycad/models/update_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="UpdateUser")
+F = TypeVar("F", bound="UpdateUser")
 
 
 @attr.s(auto_attribs=True)
 class UpdateUser:
     """The user-modifiable parts of a User."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -43,15 +43,15 @@
             field_dict["last_name"] = last_name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         discord = d.pop("discord", UNSET)
 
         first_name = d.pop("first_name", UNSET)
```

### Comparing `kittycad-0.4.2/kittycad/models/user.py` & `kittycad-0.4.3/kittycad/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-W = TypeVar("W", bound="User")
+D = TypeVar("D", bound="User")
 
 
 @attr.s(auto_attribs=True)
 class User:
     """A user."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -79,15 +79,15 @@
             field_dict["phone"] = phone
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[W], src_dict: Dict[str, Any]) -> W:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.2/kittycad/models/user_results_page.py` & `kittycad-0.4.3/kittycad/models/user_results_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="UserResultsPage")
+J = TypeVar("J", bound="UserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class UserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.user import User
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         from ..models.user import User
 
         items = cast(List[User], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.2/kittycad/models/verification_token.py` & `kittycad-0.4.3/kittycad/models/verification_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="VerificationToken")
+F = TypeVar("F", bound="VerificationToken")
 
 
 @attr.s(auto_attribs=True)
 class VerificationToken:
     """A verification token for a user.
 
     This is typically used to verify a user's email address."""  # noqa: E501
@@ -49,15 +49,15 @@
             field_dict["identifier"] = identifier
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.2/kittycad/types.py` & `kittycad-0.4.3/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.2/pyproject.toml` & `kittycad-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.4.2"
+version = "0.4.3"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
@@ -26,15 +26,15 @@
 openapi-parser = "^0.2.6"
 openapi-spec-validator = "^0.5.6"
 prance = "^0.22.11"
 pyenchant = "^3.2.2"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.269"
+ruff = "^0.0.270"
 Sphinx = "^6.2.1"
 sphinx-autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-copybutton = "^0.5.2"
 sphinxext-opengraph = "^0.8.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `kittycad-0.4.2/PKG-INFO` & `kittycad-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.4.2
+Version: 0.4.3
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/ory-client-1.1.5.tar.gz` & `tmp/ory-client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ory-client-1.1.5.tar", last modified: Wed Jan 11 13:34:03 2023, max compression
+gzip compressed data, was "dist/ory-client-1.1.7.tar", last modified: Thu Jan 26 14:15:36 2023, max compression
```

## Comparing `ory-client-1.1.5.tar` & `ory-client-1.1.7.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-11 13:29:54.000000 ory-client-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      470 2023-01-11 13:34:03.000000 ory-client-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34762 2023-01-11 13:29:54.000000 ory-client-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client/
--rw-r--r--   0 root         (0) root         (0)      835 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client/api/
--rw-r--r--   0 root         (0) root         (0)      214 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12519 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/courier_api.py
--rw-r--r--   0 root         (0) root         (0)   195774 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/frontend_api.py
--rw-r--r--   0 root         (0) root         (0)    89900 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/identity_api.py
--rw-r--r--   0 root         (0) root         (0)    40790 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/jwk_api.py
--rw-r--r--   0 root         (0) root         (0)    16180 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)   162747 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)    39826 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/oidc_api.py
--rw-r--r--   0 root         (0) root         (0)    32053 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/permission_api.py
--rw-r--r--   0 root         (0) root         (0)    70658 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/project_api.py
--rw-r--r--   0 root         (0) root         (0)    34599 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/relationship_api.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api/wellknown_api.py
--rw-r--r--   0 root         (0) root         (0)    39202 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client/apis/
--rw-r--r--   0 root         (0) root         (0)      984 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18031 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5198 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client/model/
--rw-r--r--   0 root         (0) root         (0)      344 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13971 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    13401 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)    17216 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/active_project_in_console.py
--rw-r--r--   0 root         (0) root         (0)    13840 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)    11792 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/check_opl_syntax_result.py
--rw-r--r--   0 root         (0) root         (0)    11697 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/check_permission_result.py
--rw-r--r--   0 root         (0) root         (0)    11867 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/cloud_account.py
--rw-r--r--   0 root         (0) root         (0)    12313 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/courier_message_status.py
--rw-r--r--   0 root         (0) root         (0)    12189 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/courier_message_type.py
--rw-r--r--   0 root         (0) root         (0)    12744 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)    17019 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12838 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    11720 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_project_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)    11649 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_project_body.py
--rw-r--r--   0 root         (0) root         (0)    12387 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_project_branding.py
--rw-r--r--   0 root         (0) root         (0)    12300 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_project_brandings_body.py
--rw-r--r--   0 root         (0) root         (0)    11582 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_project_invite.py
--rw-r--r--   0 root         (0) root         (0)    12513 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_recovery_code_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12510 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_recovery_link_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12810 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_relationship_body.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/create_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)    13801 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/custom_domain.py
--rw-r--r--   0 root         (0) root         (0)    12010 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/custom_domain_quota.py
--rw-r--r--   0 root         (0) root         (0)    11634 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/delete_my_sessions_count.py
--rw-r--r--   0 root         (0) root         (0)    14351 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)    14387 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/error_browser_location_change_required.py
--rw-r--r--   0 root         (0) root         (0)    14404 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/error_flow_replaced.py
--rw-r--r--   0 root         (0) root         (0)    11815 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/error_generic.py
--rw-r--r--   0 root         (0) root         (0)    12699 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)    13201 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/expanded_permission_tree.py
--rw-r--r--   0 root         (0) root         (0)    12628 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/flow_error.py
--rw-r--r--   0 root         (0) root         (0)    14404 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/generic_error.py
--rw-r--r--   0 root         (0) root         (0)    12936 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/generic_error_content.py
--rw-r--r--   0 root         (0) root         (0)    11596 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/get_managed_identity_schema_location.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11716 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/health_status.py
--rw-r--r--   0 root         (0) root         (0)    18160 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity.py
--rw-r--r--   0 root         (0) root         (0)    13621 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11911 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12545 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)    11732 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12374 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_credentials_type.py
--rw-r--r--   0 root         (0) root         (0)    12031 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_schema_container.py
--rw-r--r--   0 root         (0) root         (0)    12109 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_schema_preset.py
--rw-r--r--   0 root         (0) root         (0)    12084 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_schema_presets.py
--rw-r--r--   0 root         (0) root         (0)    12217 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    12246 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_state.py
--rw-r--r--   0 root         (0) root         (0)    12317 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11917 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12583 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)    12296 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    11957 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12226 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/identity_with_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/internal_get_project_branding_body.py
--rw-r--r--   0 root         (0) root         (0)    12439 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/internal_is_owner_for_project_by_slug_body.py
--rw-r--r--   0 root         (0) root         (0)    12039 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/internal_provision_mock_subscription.py
--rw-r--r--   0 root         (0) root         (0)    18024 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/invite_quota.py
--rw-r--r--   0 root         (0) root         (0)    12057 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/is_owner_for_project_by_slug.py
--rw-r--r--   0 root         (0) root         (0)    11628 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)    11762 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)    13081 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/json_patch.py
--rw-r--r--   0 root         (0) root         (0)    12088 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)    18000 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12346 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    11687 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/keto_namespace.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/keto_namespaces.py
--rw-r--r--   0 root         (0) root         (0)    12087 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/list_custom_domains.py
--rw-r--r--   0 root         (0) root         (0)    16881 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/login_flow.py
--rw-r--r--   0 root         (0) root         (0)    12148 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/logout_flow.py
--rw-r--r--   0 root         (0) root         (0)    13567 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/managed_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)    11792 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/managed_identity_schema_validation_result.py
--rw-r--r--   0 root         (0) root         (0)    12096 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/managed_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    16284 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/message.py
--rw-r--r--   0 root         (0) root         (0)    13688 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/message_dispatch.py
--rw-r--r--   0 root         (0) root         (0)    11555 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/namespace.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)    13825 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project.py
--rw-r--r--   0 root         (0) root         (0)   112066 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project_revision.py
--rw-r--r--   0 root         (0) root         (0)    17972 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project_revision_hook.py
--rw-r--r--   0 root         (0) root         (0)    15526 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project_revision_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)    12314 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    19781 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_project_revision_third_party_provider.py
--rw-r--r--   0 root         (0) root         (0)    12047 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/normalized_projects.py
--rw-r--r--   0 root         (0) root         (0)    11898 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/null_duration.py
--rw-r--r--   0 root         (0) root         (0)    13277 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/null_plan.py
--rw-r--r--   0 root         (0) root         (0)    37399 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)    15434 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)    18510 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    18529 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)    14919 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)    12544 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)    12229 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)    17354 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    13573 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)    13565 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)    32364 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)    24625 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)    14390 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/pagination.py
--rw-r--r--   0 root         (0) root         (0)    12222 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    12124 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/parse_error.py
--rw-r--r--   0 root         (0) root         (0)    11790 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/perform_native_logout_body.py
--rw-r--r--   0 root         (0) root         (0)    11306 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/permissions_on_project.py
--rw-r--r--   0 root         (0) root         (0)    12813 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/post_check_permission_body.py
--rw-r--r--   0 root         (0) root         (0)    12834 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/post_check_permission_or_error_body.py
--rw-r--r--   0 root         (0) root         (0)    12960 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/project.py
--rw-r--r--   0 root         (0) root         (0)    12644 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/project_api_key.py
--rw-r--r--   0 root         (0) root         (0)    12000 2023-01-11 13:29:53.000000 ory-client-1.1.5/ory_client/model/project_api_keys.py
--rw-r--r--   0 root         (0) root         (0)    13358 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_branding.py
--rw-r--r--   0 root         (0) root         (0)    23906 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_branding_colors.py
--rw-r--r--   0 root         (0) root         (0)    26077 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_branding_theme.py
--rw-r--r--   0 root         (0) root         (0)    12200 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)    12070 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_host.py
--rw-r--r--   0 root         (0) root         (0)    14551 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_invite.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_invites.py
--rw-r--r--   0 root         (0) root         (0)    11830 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_member.py
--rw-r--r--   0 root         (0) root         (0)    11995 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_members.py
--rw-r--r--   0 root         (0) root         (0)    13832 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_metadata.py
--rw-r--r--   0 root         (0) root         (0)    12032 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_metadata_list.py
--rw-r--r--   0 root         (0) root         (0)    12163 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_revision_hooks.py
--rw-r--r--   0 root         (0) root         (0)    12284 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    12348 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_revision_third_party_login_providers.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_revisions.py
--rw-r--r--   0 root         (0) root         (0)    11808 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_service_identity.py
--rw-r--r--   0 root         (0) root         (0)    11802 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_service_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)    11814 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_service_permission.py
--rw-r--r--   0 root         (0) root         (0)    12615 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/project_services.py
--rw-r--r--   0 root         (0) root         (0)    11926 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/projects.py
--rw-r--r--   0 root         (0) root         (0)    11555 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/quota_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)    12720 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/recovery_code_for_identity.py
--rw-r--r--   0 root         (0) root         (0)    15087 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)    13316 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    12615 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/recovery_identity_address.py
--rw-r--r--   0 root         (0) root         (0)    12181 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/recovery_link_for_identity.py
--rw-r--r--   0 root         (0) root         (0)    15465 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/registration_flow.py
--rw-r--r--   0 root         (0) root         (0)    13273 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)    12783 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/relation_query.py
--rw-r--r--   0 root         (0) root         (0)    13010 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/relationship.py
--rw-r--r--   0 root         (0) root         (0)    11756 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/relationship_namespaces.py
--rw-r--r--   0 root         (0) root         (0)    12062 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/relationship_patch.py
--rw-r--r--   0 root         (0) root         (0)    12258 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/relationships.py
--rw-r--r--   0 root         (0) root         (0)    12033 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/schema_patch.py
--rw-r--r--   0 root         (0) root         (0)    15254 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)    15233 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/session.py
--rw-r--r--   0 root         (0) root         (0)    12737 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)    12452 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)    11555 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/session_caching_quota.py
--rw-r--r--   0 root         (0) root         (0)    12379 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/session_device.py
--rw-r--r--   0 root         (0) root         (0)    11805 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/set_active_project_in_console_body.py
--rw-r--r--   0 root         (0) root         (0)    12735 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/set_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)    12053 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/set_project.py
--rw-r--r--   0 root         (0) root         (0)    12477 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/set_project_branding_theme_body.py
--rw-r--r--   0 root         (0) root         (0)    15402 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/settings_flow.py
--rw-r--r--   0 root         (0) root         (0)    13574 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    11710 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/source_position.py
--rw-r--r--   0 root         (0) root         (0)    11819 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)    11512 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/stripe_customer.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/subject_set.py
--rw-r--r--   0 root         (0) root         (0)    17197 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/subscription.py
--rw-r--r--   0 root         (0) root         (0)    12473 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/successful_native_login.py
--rw-r--r--   0 root         (0) root         (0)    12979 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/successful_native_registration.py
--rw-r--r--   0 root         (0) root         (0)    12962 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/successful_project_update.py
--rw-r--r--   0 root         (0) root         (0)    12880 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/token_pagination.py
--rw-r--r--   0 root         (0) root         (0)    12237 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    12930 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)    13145 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)    13912 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    14486 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    12399 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12714 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_container.py
--rw-r--r--   0 root         (0) root         (0)    14031 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node.py
--rw-r--r--   0 root         (0) root         (0)    12852 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)    22091 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12956 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)    16763 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11669 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)    14565 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12555 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11915 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)    12735 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_text.py
--rw-r--r--   0 root         (0) root         (0)    11915 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/ui_texts.py
--rw-r--r--   0 root         (0) root         (0)    14981 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    18758 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12516 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_with_lookup_secret_method.py
--rw-r--r--   0 root         (0) root         (0)    12845 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    13290 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    12404 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)    12943 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_login_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    15955 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13215 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_recovery_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)    12743 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_recovery_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)    17388 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12766 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_registration_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    12828 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_registration_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    13612 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_registration_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    21791 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13552 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_lookup_method.py
--rw-r--r--   0 root         (0) root         (0)    13168 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    12364 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    12623 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_profile_method.py
--rw-r--r--   0 root         (0) root         (0)    12887 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_settings_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    11890 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)    15152 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13137 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_verification_flow_with_code_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12769 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/update_verification_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)    13790 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)    15063 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/verification_flow.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    11586 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    11694 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model/warning.py
--rw-r--r--   0 root         (0) root         (0)    82704 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client/models/
--rw-r--r--   0 root         (0) root         (0)    16698 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14398 2023-01-11 13:29:54.000000 ory-client-1.1.5/ory_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      470 2023-01-11 13:34:02.000000 ory-client-1.1.5/ory_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18811 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 13:34:02.000000 ory-client-1.1.5/ory_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-11 13:34:03.000000 ory-client-1.1.5/ory_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-11 13:34:03.000000 ory-client-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1278 2023-01-11 13:29:54.000000 ory-client-1.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 13:34:03.000000 ory-client-1.1.5/test/
--rw-r--r--   0 root         (0) root         (0)     1279 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_active_project_in_console.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_check_opl_syntax_result.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_check_permission_result.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_cloud_account.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_courier_api.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_courier_message_status.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_courier_message_type.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_project_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_project_body.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_project_branding.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_project_brandings_body.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_project_invite.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_recovery_code_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_recovery_link_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_relationship_body.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_create_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_custom_domain.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_custom_domain_quota.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_delete_my_sessions_count.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_error_browser_location_change_required.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_error_flow_replaced.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_error_generic.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_expanded_permission_tree.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_flow_error.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_frontend_api.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_generic_error.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_generic_error_content.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_get_managed_identity_schema_location.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_health_status.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_identity_api.py
--rw-r--r--   0 root         (0) root         (0)     1049 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_credentials_type.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_schema_container.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_schema_preset.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_schema_presets.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_state.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials_oidc_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_identity_with_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_internal_get_project_branding_body.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_internal_is_owner_for_project_by_slug_body.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_internal_provision_mock_subscription.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_invite_quota.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_is_owner_for_project_by_slug.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_json_patch.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_jwk_api.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_keto_namespace.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_keto_namespaces.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_list_custom_domains.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_login_flow.py
--rw-r--r--   0 root         (0) root         (0)      844 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_logout_flow.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_managed_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_managed_identity_schema_validation_result.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_managed_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_message.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_message_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_namespace.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project.py
--rw-r--r--   0 root         (0) root         (0)     1700 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project_revision.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project_revision_hook.py
--rw-r--r--   0 root         (0) root         (0)     1184 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project_revision_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_project_revision_third_party_provider.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_normalized_projects.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_null_duration.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_null_plan.py
--rw-r--r--   0 root         (0) root         (0)     5841 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)     1350 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_oidc_api.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)      843 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_pagination.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_parse_error.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_perform_native_logout_body.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_permission_api.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_permissions_on_project.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_post_check_permission_body.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_post_check_permission_or_error_body.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_project.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_api.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_project_api_key.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-01-11 13:29:53.000000 ory-client-1.1.5/test/test_project_api_keys.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_branding.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_branding_colors.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_branding_theme.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_host.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_invite.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_invites.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_member.py
--rw-r--r--   0 root         (0) root         (0)      969 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_members.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_metadata_list.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_revision_hooks.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1276 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_revision_third_party_login_providers.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_revisions.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_service_identity.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_service_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_service_permission.py
--rw-r--r--   0 root         (0) root         (0)     1294 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_project_services.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_projects.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_quota_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_recovery_code_for_identity.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_recovery_identity_address.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_recovery_link_for_identity.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_registration_flow.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relation_query.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relationship_api.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relationship_namespaces.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relationship_patch.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_relationships.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_schema_patch.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_session.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_session_caching_quota.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_session_device.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_set_active_project_in_console_body.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_set_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_set_project.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_set_project_branding_theme_body.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_settings_flow.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_source_position.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_stripe_customer.py
--rw-r--r--   0 root         (0) root         (0)      844 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_subject_set.py
--rw-r--r--   0 root         (0) root         (0)      938 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_successful_native_login.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_successful_native_registration.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_successful_project_update.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_token_pagination.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_container.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_text.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_ui_texts.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_with_lookup_secret_method.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_login_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_recovery_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_recovery_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)     1582 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_registration_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_registration_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_registration_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1016 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_lookup_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_profile_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_settings_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_verification_flow_with_code_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_update_verification_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_verification_flow.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_warning.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-01-11 13:29:54.000000 ory-client-1.1.5/test/test_wellknown_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-01-26 14:10:08.000000 ory-client-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      470 2023-01-26 14:15:36.000000 ory-client-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34762 2023-01-26 14:10:07.000000 ory-client-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client/api/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/courier_api.py
+-rw-r--r--   0 root         (0) root         (0)   195774 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/frontend_api.py
+-rw-r--r--   0 root         (0) root         (0)    89672 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/identity_api.py
+-rw-r--r--   0 root         (0) root         (0)    40790 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)    16180 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)   162747 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)    39826 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)    32053 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/permission_api.py
+-rw-r--r--   0 root         (0) root         (0)    70658 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/project_api.py
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/relationship_api.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api/wellknown_api.py
+-rw-r--r--   0 root         (0) root         (0)    39202 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      984 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18031 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5198 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client/model/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13971 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    13401 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)    17216 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/active_project_in_console.py
+-rw-r--r--   0 root         (0) root         (0)    13840 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/check_opl_syntax_result.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/check_permission_result.py
+-rw-r--r--   0 root         (0) root         (0)    11867 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/cloud_account.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/courier_message_status.py
+-rw-r--r--   0 root         (0) root         (0)    12189 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/courier_message_type.py
+-rw-r--r--   0 root         (0) root         (0)    12744 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12838 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    11720 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_project_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)    11649 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_project_body.py
+-rw-r--r--   0 root         (0) root         (0)    12387 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)    12300 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_project_brandings_body.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_project_invite.py
+-rw-r--r--   0 root         (0) root         (0)    12513 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_recovery_code_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12510 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_recovery_link_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12810 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_relationship_body.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/create_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)    13625 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/custom_domain.py
+-rw-r--r--   0 root         (0) root         (0)    12010 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/custom_domain_quota.py
+-rw-r--r--   0 root         (0) root         (0)    11634 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/delete_my_sessions_count.py
+-rw-r--r--   0 root         (0) root         (0)    14351 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)    14387 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/error_browser_location_change_required.py
+-rw-r--r--   0 root         (0) root         (0)    14404 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/error_flow_replaced.py
+-rw-r--r--   0 root         (0) root         (0)    11815 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/error_generic.py
+-rw-r--r--   0 root         (0) root         (0)    12699 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)    13201 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/expanded_permission_tree.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/flow_error.py
+-rw-r--r--   0 root         (0) root         (0)    14404 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/generic_error.py
+-rw-r--r--   0 root         (0) root         (0)    12936 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/generic_error_content.py
+-rw-r--r--   0 root         (0) root         (0)    11596 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/get_managed_identity_schema_location.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11716 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/health_status.py
+-rw-r--r--   0 root         (0) root         (0)    18160 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity.py
+-rw-r--r--   0 root         (0) root         (0)    13621 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11911 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12545 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11732 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_credentials_type.py
+-rw-r--r--   0 root         (0) root         (0)    12031 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_schema_container.py
+-rw-r--r--   0 root         (0) root         (0)    12109 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_schema_preset.py
+-rw-r--r--   0 root         (0) root         (0)    12084 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_schema_presets.py
+-rw-r--r--   0 root         (0) root         (0)    12217 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12246 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_state.py
+-rw-r--r--   0 root         (0) root         (0)    12317 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11917 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)    12296 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12226 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/identity_with_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/internal_get_project_branding_body.py
+-rw-r--r--   0 root         (0) root         (0)    12439 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/internal_is_owner_for_project_by_slug_body.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/internal_provision_mock_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    18024 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/invite_quota.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/is_owner_for_project_by_slug.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)    13081 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/json_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12088 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)    18000 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12346 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    11687 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/keto_namespace.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/keto_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/list_custom_domains.py
+-rw-r--r--   0 root         (0) root         (0)    16881 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/login_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12148 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/logout_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13567 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/managed_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/managed_identity_schema_validation_result.py
+-rw-r--r--   0 root         (0) root         (0)    12096 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/managed_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    16284 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/message.py
+-rw-r--r--   0 root         (0) root         (0)    13688 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/message_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)    11555 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)    13825 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project.py
+-rw-r--r--   0 root         (0) root         (0)   112066 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project_revision.py
+-rw-r--r--   0 root         (0) root         (0)    17972 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project_revision_hook.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project_revision_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    19781 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_project_revision_third_party_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12047 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/normalized_projects.py
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/null_duration.py
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/null_plan.py
+-rw-r--r--   0 root         (0) root         (0)    37399 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)    15434 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)    18510 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    18529 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)    14919 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)    12544 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    17354 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    13573 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)    13565 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)    32364 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    24625 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12222 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    12124 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/parse_error.py
+-rw-r--r--   0 root         (0) root         (0)    11790 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/perform_native_logout_body.py
+-rw-r--r--   0 root         (0) root         (0)    11306 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/permissions_on_project.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/post_check_permission_body.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/post_check_permission_or_error_body.py
+-rw-r--r--   0 root         (0) root         (0)    12960 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project.py
+-rw-r--r--   0 root         (0) root         (0)    12644 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_api_key.py
+-rw-r--r--   0 root         (0) root         (0)    12000 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_api_keys.py
+-rw-r--r--   0 root         (0) root         (0)    13358 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_branding.py
+-rw-r--r--   0 root         (0) root         (0)    23906 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_branding_colors.py
+-rw-r--r--   0 root         (0) root         (0)    26077 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_branding_theme.py
+-rw-r--r--   0 root         (0) root         (0)    12200 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)    12070 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_host.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_invite.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_invites.py
+-rw-r--r--   0 root         (0) root         (0)    11830 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_member.py
+-rw-r--r--   0 root         (0) root         (0)    11995 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_members.py
+-rw-r--r--   0 root         (0) root         (0)    13832 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    12032 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_metadata_list.py
+-rw-r--r--   0 root         (0) root         (0)    12163 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_revision_hooks.py
+-rw-r--r--   0 root         (0) root         (0)    12284 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12348 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_revision_third_party_login_providers.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_revisions.py
+-rw-r--r--   0 root         (0) root         (0)    11808 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_service_identity.py
+-rw-r--r--   0 root         (0) root         (0)    11802 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_service_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)    11814 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_service_permission.py
+-rw-r--r--   0 root         (0) root         (0)    12615 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/project_services.py
+-rw-r--r--   0 root         (0) root         (0)    11926 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/projects.py
+-rw-r--r--   0 root         (0) root         (0)    11555 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/quota_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)    12720 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/recovery_code_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)    15087 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2023-01-26 14:10:06.000000 ory-client-1.1.7/ory_client/model/recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    12615 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/recovery_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/recovery_link_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)    15465 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13273 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/relation_query.py
+-rw-r--r--   0 root         (0) root         (0)    13010 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/relationship.py
+-rw-r--r--   0 root         (0) root         (0)    11756 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/relationship_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)    12062 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/relationship_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12258 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/relationships.py
+-rw-r--r--   0 root         (0) root         (0)    12033 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/schema_patch.py
+-rw-r--r--   0 root         (0) root         (0)    15254 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)    15233 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/session.py
+-rw-r--r--   0 root         (0) root         (0)    12737 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)    12452 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)    11555 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/session_caching_quota.py
+-rw-r--r--   0 root         (0) root         (0)    12379 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/session_device.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/set_active_project_in_console_body.py
+-rw-r--r--   0 root         (0) root         (0)    12735 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/set_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)    12053 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/set_project.py
+-rw-r--r--   0 root         (0) root         (0)    12477 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/set_project_branding_theme_body.py
+-rw-r--r--   0 root         (0) root         (0)    15402 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13574 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/source_position.py
+-rw-r--r--   0 root         (0) root         (0)    11819 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)    11512 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/stripe_customer.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/subject_set.py
+-rw-r--r--   0 root         (0) root         (0)    17197 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12473 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/successful_native_login.py
+-rw-r--r--   0 root         (0) root         (0)    12979 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/successful_native_registration.py
+-rw-r--r--   0 root         (0) root         (0)    12962 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/successful_project_update.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12237 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    12930 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    13145 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)    13912 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    14486 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    12399 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12714 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_container.py
+-rw-r--r--   0 root         (0) root         (0)    14031 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node.py
+-rw-r--r--   0 root         (0) root         (0)    12852 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    22091 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12956 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    16763 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11669 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)    14565 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12555 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    12735 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_text.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)    14981 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    18758 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12516 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_with_lookup_secret_method.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    13290 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    12404 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)    12943 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_login_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    15955 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13215 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_recovery_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)    12743 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_recovery_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)    17388 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12766 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_registration_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    12828 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_registration_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    13612 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_registration_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    21791 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13552 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_lookup_method.py
+-rw-r--r--   0 root         (0) root         (0)    13168 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    12364 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    12623 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_profile_method.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_settings_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    11890 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)    15152 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13137 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_verification_flow_with_code_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12769 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/update_verification_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)    13790 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)    15063 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    11586 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    11694 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model/warning.py
+-rw-r--r--   0 root         (0) root         (0)    82704 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client/models/
+-rw-r--r--   0 root         (0) root         (0)    16698 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14398 2023-01-26 14:10:07.000000 ory-client-1.1.7/ory_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-01-26 14:15:35.000000 ory-client-1.1.7/ory_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18811 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 14:15:35.000000 ory-client-1.1.7/ory_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-01-26 14:15:36.000000 ory-client-1.1.7/ory_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-26 14:15:36.000000 ory-client-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-01-26 14:10:07.000000 ory-client-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 14:15:36.000000 ory-client-1.1.7/test/
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_active_project_in_console.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_check_opl_syntax_result.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_check_permission_result.py
+-rw-r--r--   0 root         (0) root         (0)      858 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_cloud_account.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_courier_api.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_courier_message_status.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_courier_message_type.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_project_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_project_body.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_project_brandings_body.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_project_invite.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_recovery_code_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_recovery_link_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_relationship_body.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_create_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_custom_domain.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_custom_domain_quota.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_delete_my_sessions_count.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_error_browser_location_change_required.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_error_flow_replaced.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_error_generic.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_expanded_permission_tree.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_flow_error.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_frontend_api.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_generic_error.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_generic_error_content.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_get_managed_identity_schema_location.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)      858 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_health_status.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_identity_api.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_credentials_type.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_schema_container.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_schema_preset.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_schema_presets.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_state.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials_oidc_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_identity_with_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_internal_get_project_branding_body.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_internal_is_owner_for_project_by_slug_body.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_internal_provision_mock_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_invite_quota.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_is_owner_for_project_by_slug.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_json_patch.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_keto_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_keto_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_list_custom_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_login_flow.py
+-rw-r--r--   0 root         (0) root         (0)      844 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_logout_flow.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_managed_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_managed_identity_schema_validation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_managed_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_message.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_message_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project_revision.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project_revision_hook.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project_revision_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_project_revision_third_party_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_normalized_projects.py
+-rw-r--r--   0 root         (0) root         (0)      858 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_null_duration.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_null_plan.py
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)      888 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_parse_error.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_perform_native_logout_body.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_permission_api.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_permissions_on_project.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_post_check_permission_body.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_post_check_permission_or_error_body.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_project_api.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_api_key.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_api_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_branding_colors.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_branding_theme.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_host.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_invite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_invites.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_member.py
+-rw-r--r--   0 root         (0) root         (0)      969 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_members.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_metadata_list.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_revision_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_revision_third_party_login_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_revisions.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_service_identity.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_service_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_service_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_project_services.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_quota_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_recovery_code_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-01-26 14:10:06.000000 ory-client-1.1.7/test/test_recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_recovery_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_recovery_link_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relation_query.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relationship_api.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relationship_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relationship_patch.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_relationships.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_schema_patch.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_session_caching_quota.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_session_device.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_set_active_project_in_console_body.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_set_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_set_project.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_set_project_branding_theme_body.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_source_position.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_stripe_customer.py
+-rw-r--r--   0 root         (0) root         (0)      844 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_subject_set.py
+-rw-r--r--   0 root         (0) root         (0)      938 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_successful_native_login.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_successful_native_registration.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_successful_project_update.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_container.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      896 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_text.py
+-rw-r--r--   0 root         (0) root         (0)      896 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_with_lookup_secret_method.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_login_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_recovery_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_recovery_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_registration_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_registration_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_registration_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_lookup_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_profile_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_settings_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_verification_flow_with_code_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_update_verification_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_warning.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-01-26 14:10:07.000000 ory-client-1.1.7/test/test_wellknown_api.py
```

### Comparing `ory-client-1.1.5/LICENSE` & `ory-client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ory-client-1.1.5/README.md` & `ory-client-1.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ory-client
 Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed
 with a valid Personal Access Token. Public APIs are mostly used in browsers.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: v1.1.5
-- Package version: v1.1.5
+- API version: v1.1.7
+- Package version: v1.1.7
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `ory-client-1.1.5/ory_client/__init__.py` & `ory-client-1.1.7/ory_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "v1.1.5"
+__version__ = "v1.1.7"
 
 # import ApiClient
 from ory_client.api_client import ApiClient
 
 # import Configuration
 from ory_client.configuration import Configuration
```

### Comparing `ory-client-1.1.5/ory_client/api/courier_api.py` & `ory-client-1.1.7/ory_client/api/courier_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/frontend_api.py` & `ory-client-1.1.7/ory_client/api/frontend_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/identity_api.py` & `ory-client-1.1.7/ory_client/api/identity_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -535,16 +535,14 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                     ('expand',): {
 
-                        "DEVICES": "Devices",
-                        "IDENTITY": "Identity"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (str,),
                     'expand':
                         ([str],),
@@ -809,16 +807,14 @@
                         'inclusive_maximum': 1000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                     ('expand',): {
 
-                        "DEVICES": "Devices",
-                        "IDENTITY": "Identity"
                     },
                 },
                 'openapi_types': {
                     'page_size':
                         (int,),
                     'page_token':
                         (str,),
@@ -2046,15 +2042,15 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             page_size (int): Items per Page  This is the number of items per page to return. For details on pagination please head over to the [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).. [optional] if omitted the server will use the default value of 250
             page_token (str): Next Page Token  The next page token. For details on pagination please head over to the [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).. [optional]
             active (bool): Active is a boolean flag that filters out sessions based on the state. If no value is provided, all sessions are returned.. [optional]
-            expand ([str]): ExpandOptions is a query parameter encoded list of all properties that must be expanded in the Session. Example - ?expand=Identity&expand=Devices If no value is provided, the expandable properties are skipped.. [optional]
+            expand ([str]): ExpandOptions is a query parameter encoded list of all properties that must be expanded in the Session. If no value is provided, the expandable properties are skipped.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `ory-client-1.1.5/ory_client/api/jwk_api.py` & `ory-client-1.1.7/ory_client/api/jwk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/metadata_api.py` & `ory-client-1.1.7/ory_client/api/metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/o_auth2_api.py` & `ory-client-1.1.7/ory_client/api/o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/oidc_api.py` & `ory-client-1.1.7/ory_client/api/oidc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/permission_api.py` & `ory-client-1.1.7/ory_client/api/permission_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/project_api.py` & `ory-client-1.1.7/ory_client/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/relationship_api.py` & `ory-client-1.1.7/ory_client/api/relationship_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api/wellknown_api.py` & `ory-client-1.1.7/ory_client/api/wellknown_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/api_client.py` & `ory-client-1.1.7/ory_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v1.1.5/python'
+        self.user_agent = 'OpenAPI-Generator/v1.1.7/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ory-client-1.1.5/ory_client/apis/__init__.py` & `ory-client-1.1.7/ory_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-client-1.1.5/ory_client/configuration.py` & `ory-client-1.1.7/ory_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -421,16 +421,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v1.1.5\n"\
-               "SDK Package Version: v1.1.5".\
+               "Version of the API: v1.1.7\n"\
+               "SDK Package Version: v1.1.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ory-client-1.1.5/ory_client/exceptions.py` & `ory-client-1.1.7/ory_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ory-client-1.1.5/ory_client/model/accept_o_auth2_consent_request.py` & `ory-client-1.1.7/ory_client/model/accept_o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/accept_o_auth2_consent_request_session.py` & `ory-client-1.1.7/ory_client/model/accept_o_auth2_consent_request_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/accept_o_auth2_login_request.py` & `ory-client-1.1.7/ory_client/model/accept_o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/active_project_in_console.py` & `ory-client-1.1.7/ory_client/model/active_project_in_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/authenticator_assurance_level.py` & `ory-client-1.1.7/ory_client/model/authenticator_assurance_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/check_opl_syntax_result.py` & `ory-client-1.1.7/ory_client/model/check_opl_syntax_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/check_permission_result.py` & `ory-client-1.1.7/ory_client/model/check_permission_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/cloud_account.py` & `ory-client-1.1.7/ory_client/model/cloud_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/courier_message_status.py` & `ory-client-1.1.7/ory_client/model/courier_message_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/courier_message_type.py` & `ory-client-1.1.7/ory_client/model/courier_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_custom_domain_body.py` & `ory-client-1.1.7/ory_client/model/create_custom_domain_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_identity_body.py` & `ory-client-1.1.7/ory_client/model/create_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_json_web_key_set.py` & `ory-client-1.1.7/ory_client/model/create_json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_project_api_key_request.py` & `ory-client-1.1.7/ory_client/model/create_project_api_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_project_body.py` & `ory-client-1.1.7/ory_client/model/create_project_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_project_branding.py` & `ory-client-1.1.7/ory_client/model/create_project_branding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_project_brandings_body.py` & `ory-client-1.1.7/ory_client/model/create_project_brandings_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_project_invite.py` & `ory-client-1.1.7/ory_client/model/create_project_invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_recovery_code_for_identity_body.py` & `ory-client-1.1.7/ory_client/model/create_recovery_code_for_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_recovery_link_for_identity_body.py` & `ory-client-1.1.7/ory_client/model/create_recovery_link_for_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_relationship_body.py` & `ory-client-1.1.7/ory_client/model/create_relationship_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/create_subscription_body.py` & `ory-client-1.1.7/ory_client/model/create_subscription_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/custom_domain.py` & `ory-client-1.1.7/ory_client/model/custom_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -161,15 +161,15 @@
             cors_allowed_origins (StringSliceJSONFormat): [optional]  # noqa: E501
             cors_enabled (bool): [optional]  # noqa: E501
             created_at (datetime): [optional]  # noqa: E501
             hostname (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             updated_at (datetime): [optional]  # noqa: E501
             verification_errors ([str]): [optional]  # noqa: E501
-            verification_status (str): CustomHostnameStatus is the enumeration of valid state values in the CustomHostnameSSL. [optional]  # noqa: E501
+            verification_status (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,15 +255,15 @@
             cors_allowed_origins (StringSliceJSONFormat): [optional]  # noqa: E501
             cors_enabled (bool): [optional]  # noqa: E501
             created_at (datetime): [optional]  # noqa: E501
             hostname (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             updated_at (datetime): [optional]  # noqa: E501
             verification_errors ([str]): [optional]  # noqa: E501
-            verification_status (str): CustomHostnameStatus is the enumeration of valid state values in the CustomHostnameSSL. [optional]  # noqa: E501
+            verification_status (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ory-client-1.1.5/ory_client/model/custom_domain_quota.py` & `ory-client-1.1.7/ory_client/model/custom_domain_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/delete_my_sessions_count.py` & `ory-client-1.1.7/ory_client/model/delete_my_sessions_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/error_authenticator_assurance_level_not_satisfied.py` & `ory-client-1.1.7/ory_client/model/error_authenticator_assurance_level_not_satisfied.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/error_browser_location_change_required.py` & `ory-client-1.1.7/ory_client/model/error_browser_location_change_required.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/error_flow_replaced.py` & `ory-client-1.1.7/ory_client/model/error_flow_replaced.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/error_generic.py` & `ory-client-1.1.7/ory_client/model/error_generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/error_o_auth2.py` & `ory-client-1.1.7/ory_client/model/error_o_auth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/expanded_permission_tree.py` & `ory-client-1.1.7/ory_client/model/expanded_permission_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/flow_error.py` & `ory-client-1.1.7/ory_client/model/flow_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/generic_error.py` & `ory-client-1.1.7/ory_client/model/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/generic_error_content.py` & `ory-client-1.1.7/ory_client/model/generic_error_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/get_managed_identity_schema_location.py` & `ory-client-1.1.7/ory_client/model/get_managed_identity_schema_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/get_version200_response.py` & `ory-client-1.1.7/ory_client/model/get_version200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/health_not_ready_status.py` & `ory-client-1.1.7/ory_client/model/health_not_ready_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/health_status.py` & `ory-client-1.1.7/ory_client/model/health_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity.py` & `ory-client-1.1.7/ory_client/model/identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_credentials.py` & `ory-client-1.1.7/ory_client/model/identity_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_credentials_oidc.py` & `ory-client-1.1.7/ory_client/model/identity_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_credentials_oidc_provider.py` & `ory-client-1.1.7/ory_client/model/identity_credentials_oidc_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_credentials_password.py` & `ory-client-1.1.7/ory_client/model/identity_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_credentials_type.py` & `ory-client-1.1.7/ory_client/model/identity_credentials_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_schema_container.py` & `ory-client-1.1.7/ory_client/model/identity_schema_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_schema_preset.py` & `ory-client-1.1.7/ory_client/model/identity_schema_preset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_schema_presets.py` & `ory-client-1.1.7/ory_client/model/identity_schema_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_schemas.py` & `ory-client-1.1.7/ory_client/model/identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_state.py` & `ory-client-1.1.7/ory_client/model/identity_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc_config.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials_oidc_config_provider.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials_oidc_config_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials_password.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/identity_with_credentials_password_config.py` & `ory-client-1.1.7/ory_client/model/identity_with_credentials_password_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/internal_get_project_branding_body.py` & `ory-client-1.1.7/ory_client/model/internal_get_project_branding_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/internal_is_owner_for_project_by_slug_body.py` & `ory-client-1.1.7/ory_client/model/internal_is_owner_for_project_by_slug_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/internal_provision_mock_subscription.py` & `ory-client-1.1.7/ory_client/model/internal_provision_mock_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/introspected_o_auth2_token.py` & `ory-client-1.1.7/ory_client/model/introspected_o_auth2_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/invite_quota.py` & `ory-client-1.1.7/ory_client/model/invite_quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/is_owner_for_project_by_slug.py` & `ory-client-1.1.7/ory_client/model/is_owner_for_project_by_slug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/is_ready200_response.py` & `ory-client-1.1.7/ory_client/model/is_ready200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/is_ready503_response.py` & `ory-client-1.1.7/ory_client/model/is_ready503_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/json_patch.py` & `ory-client-1.1.7/ory_client/model/json_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/json_patch_document.py` & `ory-client-1.1.7/ory_client/model/json_patch_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/json_web_key.py` & `ory-client-1.1.7/ory_client/model/json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/json_web_key_set.py` & `ory-client-1.1.7/ory_client/model/json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/keto_namespace.py` & `ory-client-1.1.7/ory_client/model/keto_namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/keto_namespaces.py` & `ory-client-1.1.7/ory_client/model/keto_namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/list_custom_domains.py` & `ory-client-1.1.7/ory_client/model/list_custom_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/login_flow.py` & `ory-client-1.1.7/ory_client/model/login_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/logout_flow.py` & `ory-client-1.1.7/ory_client/model/logout_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/managed_identity_schema.py` & `ory-client-1.1.7/ory_client/model/managed_identity_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/managed_identity_schema_validation_result.py` & `ory-client-1.1.7/ory_client/model/managed_identity_schema_validation_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/managed_identity_schemas.py` & `ory-client-1.1.7/ory_client/model/managed_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/message.py` & `ory-client-1.1.7/ory_client/model/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/message_dispatch.py` & `ory-client-1.1.7/ory_client/model/message_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/namespace.py` & `ory-client-1.1.7/ory_client/model/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/needs_privileged_session_error.py` & `ory-client-1.1.7/ory_client/model/needs_privileged_session_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project.py` & `ory-client-1.1.7/ory_client/model/normalized_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project_revision.py` & `ory-client-1.1.7/ory_client/model/normalized_project_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project_revision_hook.py` & `ory-client-1.1.7/ory_client/model/normalized_project_revision_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project_revision_identity_schema.py` & `ory-client-1.1.7/ory_client/model/normalized_project_revision_identity_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project_revision_identity_schemas.py` & `ory-client-1.1.7/ory_client/model/normalized_project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_project_revision_third_party_provider.py` & `ory-client-1.1.7/ory_client/model/normalized_project_revision_third_party_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/normalized_projects.py` & `ory-client-1.1.7/ory_client/model/normalized_projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/null_duration.py` & `ory-client-1.1.7/ory_client/model/null_duration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/null_plan.py` & `ory-client-1.1.7/ory_client/model/null_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_client.py` & `ory-client-1.1.7/ory_client/model/o_auth2_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_client_token_lifespans.py` & `ory-client-1.1.7/ory_client/model/o_auth2_client_token_lifespans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_consent_request.py` & `ory-client-1.1.7/ory_client/model/o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_consent_request_open_id_connect_context.py` & `ory-client-1.1.7/ory_client/model/o_auth2_consent_request_open_id_connect_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_consent_session.py` & `ory-client-1.1.7/ory_client/model/o_auth2_consent_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_consent_session_expires_at.py` & `ory-client-1.1.7/ory_client/model/o_auth2_consent_session_expires_at.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_consent_sessions.py` & `ory-client-1.1.7/ory_client/model/o_auth2_consent_sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_login_request.py` & `ory-client-1.1.7/ory_client/model/o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_logout_request.py` & `ory-client-1.1.7/ory_client/model/o_auth2_logout_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_redirect_to.py` & `ory-client-1.1.7/ory_client/model/o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/o_auth2_token_exchange.py` & `ory-client-1.1.7/ory_client/model/o_auth2_token_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/oidc_configuration.py` & `ory-client-1.1.7/ory_client/model/oidc_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/oidc_user_info.py` & `ory-client-1.1.7/ory_client/model/oidc_user_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/pagination.py` & `ory-client-1.1.7/ory_client/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/pagination_headers.py` & `ory-client-1.1.7/ory_client/model/pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/parse_error.py` & `ory-client-1.1.7/ory_client/model/parse_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/perform_native_logout_body.py` & `ory-client-1.1.7/ory_client/model/perform_native_logout_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/permissions_on_project.py` & `ory-client-1.1.7/ory_client/model/permissions_on_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/post_check_permission_body.py` & `ory-client-1.1.7/ory_client/model/post_check_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/post_check_permission_or_error_body.py` & `ory-client-1.1.7/ory_client/model/post_check_permission_or_error_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project.py` & `ory-client-1.1.7/ory_client/model/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_api_key.py` & `ory-client-1.1.7/ory_client/model/project_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_api_keys.py` & `ory-client-1.1.7/ory_client/model/project_api_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_branding.py` & `ory-client-1.1.7/ory_client/model/project_branding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_branding_colors.py` & `ory-client-1.1.7/ory_client/model/project_branding_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_branding_theme.py` & `ory-client-1.1.7/ory_client/model/project_branding_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_branding_themes.py` & `ory-client-1.1.7/ory_client/model/project_branding_themes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_host.py` & `ory-client-1.1.7/ory_client/model/project_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_invite.py` & `ory-client-1.1.7/ory_client/model/project_invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_invites.py` & `ory-client-1.1.7/ory_client/model/project_invites.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_member.py` & `ory-client-1.1.7/ory_client/model/project_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_members.py` & `ory-client-1.1.7/ory_client/model/project_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_metadata.py` & `ory-client-1.1.7/ory_client/model/project_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_metadata_list.py` & `ory-client-1.1.7/ory_client/model/project_metadata_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_revision_hooks.py` & `ory-client-1.1.7/ory_client/model/project_revision_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_revision_identity_schemas.py` & `ory-client-1.1.7/ory_client/model/project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_revision_third_party_login_providers.py` & `ory-client-1.1.7/ory_client/model/project_revision_third_party_login_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_revisions.py` & `ory-client-1.1.7/ory_client/model/project_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_service_identity.py` & `ory-client-1.1.7/ory_client/model/project_service_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_service_o_auth2.py` & `ory-client-1.1.7/ory_client/model/project_service_o_auth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_service_permission.py` & `ory-client-1.1.7/ory_client/model/project_service_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/project_services.py` & `ory-client-1.1.7/ory_client/model/project_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/projects.py` & `ory-client-1.1.7/ory_client/model/projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/quota_branding_themes.py` & `ory-client-1.1.7/ory_client/model/quota_branding_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/recovery_code_for_identity.py` & `ory-client-1.1.7/ory_client/model/recovery_code_for_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/recovery_flow.py` & `ory-client-1.1.7/ory_client/model/recovery_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/recovery_flow_state.py` & `ory-client-1.1.7/ory_client/model/recovery_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/recovery_identity_address.py` & `ory-client-1.1.7/ory_client/model/recovery_identity_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/recovery_link_for_identity.py` & `ory-client-1.1.7/ory_client/model/recovery_link_for_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/registration_flow.py` & `ory-client-1.1.7/ory_client/model/registration_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/reject_o_auth2_request.py` & `ory-client-1.1.7/ory_client/model/reject_o_auth2_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/relation_query.py` & `ory-client-1.1.7/ory_client/model/relation_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/relationship.py` & `ory-client-1.1.7/ory_client/model/relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/relationship_namespaces.py` & `ory-client-1.1.7/ory_client/model/relationship_namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/relationship_patch.py` & `ory-client-1.1.7/ory_client/model/relationship_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/relationships.py` & `ory-client-1.1.7/ory_client/model/relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/schema_patch.py` & `ory-client-1.1.7/ory_client/model/schema_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/self_service_flow_expired_error.py` & `ory-client-1.1.7/ory_client/model/self_service_flow_expired_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/session.py` & `ory-client-1.1.7/ory_client/model/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/session_authentication_method.py` & `ory-client-1.1.7/ory_client/model/session_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/session_authentication_methods.py` & `ory-client-1.1.7/ory_client/model/session_authentication_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/session_caching_quota.py` & `ory-client-1.1.7/ory_client/model/session_caching_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/session_device.py` & `ory-client-1.1.7/ory_client/model/session_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/set_active_project_in_console_body.py` & `ory-client-1.1.7/ory_client/model/set_active_project_in_console_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/set_custom_domain_body.py` & `ory-client-1.1.7/ory_client/model/set_custom_domain_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/set_project.py` & `ory-client-1.1.7/ory_client/model/set_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/set_project_branding_theme_body.py` & `ory-client-1.1.7/ory_client/model/set_project_branding_theme_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/settings_flow.py` & `ory-client-1.1.7/ory_client/model/settings_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/settings_flow_state.py` & `ory-client-1.1.7/ory_client/model/settings_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/source_position.py` & `ory-client-1.1.7/ory_client/model/source_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/string_slice_json_format.py` & `ory-client-1.1.7/ory_client/model/string_slice_json_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/stripe_customer.py` & `ory-client-1.1.7/ory_client/model/stripe_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/subject_set.py` & `ory-client-1.1.7/ory_client/model/subject_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/subscription.py` & `ory-client-1.1.7/ory_client/model/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/successful_native_login.py` & `ory-client-1.1.7/ory_client/model/successful_native_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/successful_native_registration.py` & `ory-client-1.1.7/ory_client/model/successful_native_registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/successful_project_update.py` & `ory-client-1.1.7/ory_client/model/successful_project_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/token_pagination.py` & `ory-client-1.1.7/ory_client/model/token_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/token_pagination_headers.py` & `ory-client-1.1.7/ory_client/model/token_pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/token_pagination_request_parameters.py` & `ory-client-1.1.7/ory_client/model/token_pagination_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/token_pagination_response_headers.py` & `ory-client-1.1.7/ory_client/model/token_pagination_response_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/trust_o_auth2_jwt_grant_issuer.py` & `ory-client-1.1.7/ory_client/model/trust_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py` & `ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py` & `ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-client-1.1.7/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_container.py` & `ory-client-1.1.7/ory_client/model/ui_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node.py` & `ory-client-1.1.7/ory_client/model/ui_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_anchor_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_anchor_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_image_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_image_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_input_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_input_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_meta.py` & `ory-client-1.1.7/ory_client/model/ui_node_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_script_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_script_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_node_text_attributes.py` & `ory-client-1.1.7/ory_client/model/ui_node_text_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_nodes.py` & `ory-client-1.1.7/ory_client/model/ui_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_text.py` & `ory-client-1.1.7/ory_client/model/ui_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/ui_texts.py` & `ory-client-1.1.7/ory_client/model/ui_texts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_identity_body.py` & `ory-client-1.1.7/ory_client/model/update_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_body.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_with_lookup_secret_method.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_with_lookup_secret_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_with_oidc_method.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_with_password_method.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_with_totp_method.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_with_totp_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_login_flow_with_web_authn_method.py` & `ory-client-1.1.7/ory_client/model/update_login_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_recovery_flow_body.py` & `ory-client-1.1.7/ory_client/model/update_recovery_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_recovery_flow_with_code_method.py` & `ory-client-1.1.7/ory_client/model/update_recovery_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_recovery_flow_with_link_method.py` & `ory-client-1.1.7/ory_client/model/update_recovery_flow_with_link_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_registration_flow_body.py` & `ory-client-1.1.7/ory_client/model/update_registration_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_registration_flow_with_oidc_method.py` & `ory-client-1.1.7/ory_client/model/update_registration_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_registration_flow_with_password_method.py` & `ory-client-1.1.7/ory_client/model/update_registration_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_registration_flow_with_web_authn_method.py` & `ory-client-1.1.7/ory_client/model/update_registration_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_body.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_lookup_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_lookup_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_oidc_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_password_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_profile_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_profile_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_totp_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_totp_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_settings_flow_with_web_authn_method.py` & `ory-client-1.1.7/ory_client/model/update_settings_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_subscription_body.py` & `ory-client-1.1.7/ory_client/model/update_subscription_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_verification_flow_body.py` & `ory-client-1.1.7/ory_client/model/update_verification_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_verification_flow_with_code_method_body.py` & `ory-client-1.1.7/ory_client/model/update_verification_flow_with_code_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/update_verification_flow_with_link_method.py` & `ory-client-1.1.7/ory_client/model/update_verification_flow_with_link_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/verifiable_identity_address.py` & `ory-client-1.1.7/ory_client/model/verifiable_identity_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/verification_flow.py` & `ory-client-1.1.7/ory_client/model/verification_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/verification_flow_state.py` & `ory-client-1.1.7/ory_client/model/verification_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/version.py` & `ory-client-1.1.7/ory_client/model/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model/warning.py` & `ory-client-1.1.7/ory_client/model/warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.1.5/ory_client/model_utils.py` & `ory-client-1.1.7/ory_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `ory-client-1.1.5/ory_client/models/__init__.py` & `ory-client-1.1.7/ory_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-client-1.1.5/ory_client/rest.py` & `ory-client-1.1.7/ory_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `ory-client-1.1.5/ory_client.egg-info/SOURCES.txt` & `ory-client-1.1.7/ory_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ory-client-1.1.5/setup.py` & `ory-client-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ory-client"
-VERSION = "v1.1.5"
+VERSION = "v1.1.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ory-client-1.1.5/test/test_accept_o_auth2_consent_request.py` & `ory-client-1.1.7/test/test_accept_o_auth2_consent_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_accept_o_auth2_consent_request_session.py` & `ory-client-1.1.7/test/test_accept_o_auth2_consent_request_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_accept_o_auth2_login_request.py` & `ory-client-1.1.7/test/test_accept_o_auth2_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_active_project_in_console.py` & `ory-client-1.1.7/test/test_active_project_in_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_authenticator_assurance_level.py` & `ory-client-1.1.7/test/test_authenticator_assurance_level.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_check_opl_syntax_result.py` & `ory-client-1.1.7/test/test_check_opl_syntax_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_check_permission_result.py` & `ory-client-1.1.7/test/test_check_permission_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_cloud_account.py` & `ory-client-1.1.7/test/test_cloud_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_courier_api.py` & `ory-client-1.1.7/test/test_courier_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_courier_message_status.py` & `ory-client-1.1.7/test/test_courier_message_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_courier_message_type.py` & `ory-client-1.1.7/test/test_courier_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_custom_domain_body.py` & `ory-client-1.1.7/test/test_create_custom_domain_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_identity_body.py` & `ory-client-1.1.7/test/test_create_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_json_web_key_set.py` & `ory-client-1.1.7/test/test_create_json_web_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_project_api_key_request.py` & `ory-client-1.1.7/test/test_create_project_api_key_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_project_body.py` & `ory-client-1.1.7/test/test_create_project_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_project_branding.py` & `ory-client-1.1.7/test/test_create_project_branding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_project_brandings_body.py` & `ory-client-1.1.7/test/test_create_project_brandings_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_project_invite.py` & `ory-client-1.1.7/test/test_create_project_invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_recovery_code_for_identity_body.py` & `ory-client-1.1.7/test/test_create_recovery_code_for_identity_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_recovery_link_for_identity_body.py` & `ory-client-1.1.7/test/test_create_recovery_link_for_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_relationship_body.py` & `ory-client-1.1.7/test/test_create_relationship_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_create_subscription_body.py` & `ory-client-1.1.7/test/test_create_subscription_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_custom_domain.py` & `ory-client-1.1.7/test/test_custom_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_custom_domain_quota.py` & `ory-client-1.1.7/test/test_custom_domain_quota.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_delete_my_sessions_count.py` & `ory-client-1.1.7/test/test_delete_my_sessions_count.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_error_authenticator_assurance_level_not_satisfied.py` & `ory-client-1.1.7/test/test_error_authenticator_assurance_level_not_satisfied.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_error_browser_location_change_required.py` & `ory-client-1.1.7/test/test_error_browser_location_change_required.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_error_flow_replaced.py` & `ory-client-1.1.7/test/test_error_flow_replaced.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_error_generic.py` & `ory-client-1.1.7/test/test_error_generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_error_o_auth2.py` & `ory-client-1.1.7/test/test_error_o_auth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_expanded_permission_tree.py` & `ory-client-1.1.7/test/test_expanded_permission_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_flow_error.py` & `ory-client-1.1.7/test/test_flow_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_frontend_api.py` & `ory-client-1.1.7/test/test_frontend_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_generic_error.py` & `ory-client-1.1.7/test/test_generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_generic_error_content.py` & `ory-client-1.1.7/test/test_generic_error_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_get_managed_identity_schema_location.py` & `ory-client-1.1.7/test/test_get_managed_identity_schema_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_get_version200_response.py` & `ory-client-1.1.7/test/test_get_version200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_health_not_ready_status.py` & `ory-client-1.1.7/test/test_health_not_ready_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_health_status.py` & `ory-client-1.1.7/test/test_health_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity.py` & `ory-client-1.1.7/test/test_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_api.py` & `ory-client-1.1.7/test/test_identity_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_credentials.py` & `ory-client-1.1.7/test/test_identity_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_credentials_oidc.py` & `ory-client-1.1.7/test/test_identity_credentials_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_credentials_oidc_provider.py` & `ory-client-1.1.7/test/test_identity_credentials_oidc_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_credentials_password.py` & `ory-client-1.1.7/test/test_identity_credentials_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_credentials_type.py` & `ory-client-1.1.7/test/test_identity_credentials_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_schema_container.py` & `ory-client-1.1.7/test/test_identity_schema_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_schema_preset.py` & `ory-client-1.1.7/test/test_identity_schema_presets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
 from ory_client.model.identity_schema_preset import IdentitySchemaPreset
+globals()['IdentitySchemaPreset'] = IdentitySchemaPreset
+from ory_client.model.identity_schema_presets import IdentitySchemaPresets
 
 
-class TestIdentitySchemaPreset(unittest.TestCase):
-    """IdentitySchemaPreset unit test stubs"""
+class TestIdentitySchemaPresets(unittest.TestCase):
+    """IdentitySchemaPresets unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemaPreset(self):
-        """Test IdentitySchemaPreset"""
+    def testIdentitySchemaPresets(self):
+        """Test IdentitySchemaPresets"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemaPreset()  # noqa: E501
+        # model = IdentitySchemaPresets()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_schema_presets.py` & `ory-client-1.1.7/test/test_identity_schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_schema_preset import IdentitySchemaPreset
-globals()['IdentitySchemaPreset'] = IdentitySchemaPreset
-from ory_client.model.identity_schema_presets import IdentitySchemaPresets
+from ory_client.model.identity_schema_container import IdentitySchemaContainer
+globals()['IdentitySchemaContainer'] = IdentitySchemaContainer
+from ory_client.model.identity_schemas import IdentitySchemas
 
 
-class TestIdentitySchemaPresets(unittest.TestCase):
-    """IdentitySchemaPresets unit test stubs"""
+class TestIdentitySchemas(unittest.TestCase):
+    """IdentitySchemas unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemaPresets(self):
-        """Test IdentitySchemaPresets"""
+    def testIdentitySchemas(self):
+        """Test IdentitySchemas"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemaPresets()  # noqa: E501
+        # model = IdentitySchemas()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_schemas.py` & `ory-client-1.1.7/test/test_managed_identity_schema_validation_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_schema_container import IdentitySchemaContainer
-globals()['IdentitySchemaContainer'] = IdentitySchemaContainer
-from ory_client.model.identity_schemas import IdentitySchemas
+from ory_client.model.managed_identity_schema_validation_result import ManagedIdentitySchemaValidationResult
 
 
-class TestIdentitySchemas(unittest.TestCase):
-    """IdentitySchemas unit test stubs"""
+class TestManagedIdentitySchemaValidationResult(unittest.TestCase):
+    """ManagedIdentitySchemaValidationResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemas(self):
-        """Test IdentitySchemas"""
+    def testManagedIdentitySchemaValidationResult(self):
+        """Test ManagedIdentitySchemaValidationResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemas()  # noqa: E501
+        # model = ManagedIdentitySchemaValidationResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_state.py` & `ory-client-1.1.7/test/test_identity_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials.py` & `ory-client-1.1.7/test/test_identity_with_credentials_oidc_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_with_credentials_oidc import IdentityWithCredentialsOidc
-from ory_client.model.identity_with_credentials_password import IdentityWithCredentialsPassword
-globals()['IdentityWithCredentialsOidc'] = IdentityWithCredentialsOidc
-globals()['IdentityWithCredentialsPassword'] = IdentityWithCredentialsPassword
-from ory_client.model.identity_with_credentials import IdentityWithCredentials
+from ory_client.model.identity_with_credentials_oidc_config_provider import IdentityWithCredentialsOidcConfigProvider
+from ory_client.model.identity_with_credentials_password_config import IdentityWithCredentialsPasswordConfig
+globals()['IdentityWithCredentialsOidcConfigProvider'] = IdentityWithCredentialsOidcConfigProvider
+globals()['IdentityWithCredentialsPasswordConfig'] = IdentityWithCredentialsPasswordConfig
+from ory_client.model.identity_with_credentials_oidc_config import IdentityWithCredentialsOidcConfig
 
 
-class TestIdentityWithCredentials(unittest.TestCase):
-    """IdentityWithCredentials unit test stubs"""
+class TestIdentityWithCredentialsOidcConfig(unittest.TestCase):
+    """IdentityWithCredentialsOidcConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentityWithCredentials(self):
-        """Test IdentityWithCredentials"""
+    def testIdentityWithCredentialsOidcConfig(self):
+        """Test IdentityWithCredentialsOidcConfig"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentityWithCredentials()  # noqa: E501
+        # model = IdentityWithCredentialsOidcConfig()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials_oidc.py` & `ory-client-1.1.7/test/test_identity_with_credentials_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials_oidc_config.py` & `ory-client-1.1.7/test/test_identity_with_credentials_password.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_with_credentials_oidc_config_provider import IdentityWithCredentialsOidcConfigProvider
 from ory_client.model.identity_with_credentials_password_config import IdentityWithCredentialsPasswordConfig
-globals()['IdentityWithCredentialsOidcConfigProvider'] = IdentityWithCredentialsOidcConfigProvider
 globals()['IdentityWithCredentialsPasswordConfig'] = IdentityWithCredentialsPasswordConfig
-from ory_client.model.identity_with_credentials_oidc_config import IdentityWithCredentialsOidcConfig
+from ory_client.model.identity_with_credentials_password import IdentityWithCredentialsPassword
 
 
-class TestIdentityWithCredentialsOidcConfig(unittest.TestCase):
-    """IdentityWithCredentialsOidcConfig unit test stubs"""
+class TestIdentityWithCredentialsPassword(unittest.TestCase):
+    """IdentityWithCredentialsPassword unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentityWithCredentialsOidcConfig(self):
-        """Test IdentityWithCredentialsOidcConfig"""
+    def testIdentityWithCredentialsPassword(self):
+        """Test IdentityWithCredentialsPassword"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentityWithCredentialsOidcConfig()  # noqa: E501
+        # model = IdentityWithCredentialsPassword()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials_oidc_config_provider.py` & `ory-client-1.1.7/test/test_identity_with_credentials_oidc_config_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials_password.py` & `ory-client-1.1.7/test/test_managed_identity_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_with_credentials_password_config import IdentityWithCredentialsPasswordConfig
-globals()['IdentityWithCredentialsPasswordConfig'] = IdentityWithCredentialsPasswordConfig
-from ory_client.model.identity_with_credentials_password import IdentityWithCredentialsPassword
+from ory_client.model.managed_identity_schema import ManagedIdentitySchema
 
 
-class TestIdentityWithCredentialsPassword(unittest.TestCase):
-    """IdentityWithCredentialsPassword unit test stubs"""
+class TestManagedIdentitySchema(unittest.TestCase):
+    """ManagedIdentitySchema unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentityWithCredentialsPassword(self):
-        """Test IdentityWithCredentialsPassword"""
+    def testManagedIdentitySchema(self):
+        """Test ManagedIdentitySchema"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentityWithCredentialsPassword()  # noqa: E501
+        # model = ManagedIdentitySchema()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_identity_with_credentials_password_config.py` & `ory-client-1.1.7/test/test_identity_with_credentials_password_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_internal_get_project_branding_body.py` & `ory-client-1.1.7/test/test_internal_get_project_branding_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_internal_is_owner_for_project_by_slug_body.py` & `ory-client-1.1.7/test/test_internal_is_owner_for_project_by_slug_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_internal_provision_mock_subscription.py` & `ory-client-1.1.7/test/test_internal_provision_mock_subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_introspected_o_auth2_token.py` & `ory-client-1.1.7/test/test_introspected_o_auth2_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_invite_quota.py` & `ory-client-1.1.7/test/test_invite_quota.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_is_owner_for_project_by_slug.py` & `ory-client-1.1.7/test/test_is_owner_for_project_by_slug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_is_ready200_response.py` & `ory-client-1.1.7/test/test_is_ready503_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.is_ready200_response import IsReady200Response
+from ory_client.model.is_ready503_response import IsReady503Response
 
 
-class TestIsReady200Response(unittest.TestCase):
-    """IsReady200Response unit test stubs"""
+class TestIsReady503Response(unittest.TestCase):
+    """IsReady503Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIsReady200Response(self):
-        """Test IsReady200Response"""
+    def testIsReady503Response(self):
+        """Test IsReady503Response"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IsReady200Response()  # noqa: E501
+        # model = IsReady503Response()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_is_ready503_response.py` & `ory-client-1.1.7/test/test_is_ready200_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.is_ready503_response import IsReady503Response
+from ory_client.model.is_ready200_response import IsReady200Response
 
 
-class TestIsReady503Response(unittest.TestCase):
-    """IsReady503Response unit test stubs"""
+class TestIsReady200Response(unittest.TestCase):
+    """IsReady200Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIsReady503Response(self):
-        """Test IsReady503Response"""
+    def testIsReady200Response(self):
+        """Test IsReady200Response"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IsReady503Response()  # noqa: E501
+        # model = IsReady200Response()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_json_patch.py` & `ory-client-1.1.7/test/test_json_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_json_patch_document.py` & `ory-client-1.1.7/test/test_json_patch_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_json_web_key.py` & `ory-client-1.1.7/test/test_json_web_key.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_json_web_key_set.py` & `ory-client-1.1.7/test/test_json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_jwk_api.py` & `ory-client-1.1.7/test/test_jwk_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_keto_namespace.py` & `ory-client-1.1.7/test/test_keto_namespace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_keto_namespaces.py` & `ory-client-1.1.7/test/test_keto_namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_list_custom_domains.py` & `ory-client-1.1.7/test/test_list_custom_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_login_flow.py` & `ory-client-1.1.7/test/test_login_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_logout_flow.py` & `ory-client-1.1.7/test/test_logout_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_managed_identity_schema.py` & `ory-client-1.1.7/test/test_schema_patch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.managed_identity_schema import ManagedIdentitySchema
+from ory_client.model.schema_patch import SchemaPatch
 
 
-class TestManagedIdentitySchema(unittest.TestCase):
-    """ManagedIdentitySchema unit test stubs"""
+class TestSchemaPatch(unittest.TestCase):
+    """SchemaPatch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testManagedIdentitySchema(self):
-        """Test ManagedIdentitySchema"""
+    def testSchemaPatch(self):
+        """Test SchemaPatch"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ManagedIdentitySchema()  # noqa: E501
+        # model = SchemaPatch()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_managed_identity_schema_validation_result.py` & `ory-client-1.1.7/test/test_settings_flow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.managed_identity_schema_validation_result import ManagedIdentitySchemaValidationResult
+from ory_client.model.identity import Identity
+from ory_client.model.settings_flow_state import SettingsFlowState
+from ory_client.model.ui_container import UiContainer
+globals()['Identity'] = Identity
+globals()['SettingsFlowState'] = SettingsFlowState
+globals()['UiContainer'] = UiContainer
+from ory_client.model.settings_flow import SettingsFlow
 
 
-class TestManagedIdentitySchemaValidationResult(unittest.TestCase):
-    """ManagedIdentitySchemaValidationResult unit test stubs"""
+class TestSettingsFlow(unittest.TestCase):
+    """SettingsFlow unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testManagedIdentitySchemaValidationResult(self):
-        """Test ManagedIdentitySchemaValidationResult"""
+    def testSettingsFlow(self):
+        """Test SettingsFlow"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ManagedIdentitySchemaValidationResult()  # noqa: E501
+        # model = SettingsFlow()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_managed_identity_schemas.py` & `ory-client-1.1.7/test/test_managed_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_message.py` & `ory-client-1.1.7/test/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_message_dispatch.py` & `ory-client-1.1.7/test/test_message_dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_metadata_api.py` & `ory-client-1.1.7/test/test_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_namespace.py` & `ory-client-1.1.7/test/test_namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_needs_privileged_session_error.py` & `ory-client-1.1.7/test/test_needs_privileged_session_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project.py` & `ory-client-1.1.7/test/test_normalized_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project_revision.py` & `ory-client-1.1.7/test/test_normalized_project_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project_revision_hook.py` & `ory-client-1.1.7/test/test_normalized_project_revision_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project_revision_identity_schema.py` & `ory-client-1.1.7/test/test_normalized_project_revision_identity_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project_revision_identity_schemas.py` & `ory-client-1.1.7/test/test_normalized_project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_project_revision_third_party_provider.py` & `ory-client-1.1.7/test/test_normalized_project_revision_third_party_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_normalized_projects.py` & `ory-client-1.1.7/test/test_normalized_projects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_null_duration.py` & `ory-client-1.1.7/test/test_null_duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_null_plan.py` & `ory-client-1.1.7/test/test_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.null_plan import NullPlan
+from ory_client.model.version import Version
 
 
-class TestNullPlan(unittest.TestCase):
-    """NullPlan unit test stubs"""
+class TestVersion(unittest.TestCase):
+    """Version unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNullPlan(self):
-        """Test NullPlan"""
+    def testVersion(self):
+        """Test Version"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = NullPlan()  # noqa: E501
+        # model = Version()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_api.py` & `ory-client-1.1.7/test/test_o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_client.py` & `ory-client-1.1.7/test/test_o_auth2_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_client_token_lifespans.py` & `ory-client-1.1.7/test/test_o_auth2_client_token_lifespans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_consent_request.py` & `ory-client-1.1.7/test/test_o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_consent_request_open_id_connect_context.py` & `ory-client-1.1.7/test/test_o_auth2_consent_request_open_id_connect_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_consent_session.py` & `ory-client-1.1.7/test/test_o_auth2_consent_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_consent_session_expires_at.py` & `ory-client-1.1.7/test/test_o_auth2_consent_session_expires_at.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_consent_sessions.py` & `ory-client-1.1.7/test/test_o_auth2_consent_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_login_request.py` & `ory-client-1.1.7/test/test_o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_logout_request.py` & `ory-client-1.1.7/test/test_o_auth2_logout_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_redirect_to.py` & `ory-client-1.1.7/test/test_o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_o_auth2_token_exchange.py` & `ory-client-1.1.7/test/test_o_auth2_token_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_oidc_api.py` & `ory-client-1.1.7/test/test_oidc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_oidc_configuration.py` & `ory-client-1.1.7/test/test_oidc_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_oidc_user_info.py` & `ory-client-1.1.7/test/test_oidc_user_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_pagination.py` & `ory-client-1.1.7/test/test_token_pagination.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.pagination import Pagination
+from ory_client.model.token_pagination import TokenPagination
 
 
-class TestPagination(unittest.TestCase):
-    """Pagination unit test stubs"""
+class TestTokenPagination(unittest.TestCase):
+    """TokenPagination unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPagination(self):
-        """Test Pagination"""
+    def testTokenPagination(self):
+        """Test TokenPagination"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Pagination()  # noqa: E501
+        # model = TokenPagination()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_pagination_headers.py` & `ory-client-1.1.7/test/test_pagination_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_parse_error.py` & `ory-client-1.1.7/test/test_parse_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_perform_native_logout_body.py` & `ory-client-1.1.7/test/test_perform_native_logout_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_permission_api.py` & `ory-client-1.1.7/test/test_permission_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_permissions_on_project.py` & `ory-client-1.1.7/test/test_project_service_identity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.permissions_on_project import PermissionsOnProject
+from ory_client.model.project_service_identity import ProjectServiceIdentity
 
 
-class TestPermissionsOnProject(unittest.TestCase):
-    """PermissionsOnProject unit test stubs"""
+class TestProjectServiceIdentity(unittest.TestCase):
+    """ProjectServiceIdentity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPermissionsOnProject(self):
-        """Test PermissionsOnProject"""
+    def testProjectServiceIdentity(self):
+        """Test ProjectServiceIdentity"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PermissionsOnProject()  # noqa: E501
+        # model = ProjectServiceIdentity()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_post_check_permission_body.py` & `ory-client-1.1.7/test/test_post_check_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_post_check_permission_or_error_body.py` & `ory-client-1.1.7/test/test_post_check_permission_or_error_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project.py` & `ory-client-1.1.7/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_api.py` & `ory-client-1.1.7/test/test_project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_api_key.py` & `ory-client-1.1.7/test/test_project_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_api_keys.py` & `ory-client-1.1.7/test/test_project_api_keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_branding.py` & `ory-client-1.1.7/test/test_project_branding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_branding_colors.py` & `ory-client-1.1.7/test/test_project_branding_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_branding_theme.py` & `ory-client-1.1.7/test/test_project_branding_theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_branding_themes.py` & `ory-client-1.1.7/test/test_project_branding_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_host.py` & `ory-client-1.1.7/test/test_project_host.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_invite.py` & `ory-client-1.1.7/test/test_project_invite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_invites.py` & `ory-client-1.1.7/test/test_project_invites.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_member.py` & `ory-client-1.1.7/test/test_project_member.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_members.py` & `ory-client-1.1.7/test/test_project_members.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_metadata.py` & `ory-client-1.1.7/test/test_project_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_metadata_list.py` & `ory-client-1.1.7/test/test_project_metadata_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_revision_hooks.py` & `ory-client-1.1.7/test/test_project_revision_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_revision_identity_schemas.py` & `ory-client-1.1.7/test/test_project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_revision_third_party_login_providers.py` & `ory-client-1.1.7/test/test_project_revision_third_party_login_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_revisions.py` & `ory-client-1.1.7/test/test_project_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_project_service_identity.py` & `ory-client-1.1.7/test/test_project_service_o_auth2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_service_identity import ProjectServiceIdentity
+from ory_client.model.project_service_o_auth2 import ProjectServiceOAuth2
 
 
-class TestProjectServiceIdentity(unittest.TestCase):
-    """ProjectServiceIdentity unit test stubs"""
+class TestProjectServiceOAuth2(unittest.TestCase):
+    """ProjectServiceOAuth2 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectServiceIdentity(self):
-        """Test ProjectServiceIdentity"""
+    def testProjectServiceOAuth2(self):
+        """Test ProjectServiceOAuth2"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectServiceIdentity()  # noqa: E501
+        # model = ProjectServiceOAuth2()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_project_service_o_auth2.py` & `ory-client-1.1.7/test/test_project_service_permission.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_service_o_auth2 import ProjectServiceOAuth2
+from ory_client.model.project_service_permission import ProjectServicePermission
 
 
-class TestProjectServiceOAuth2(unittest.TestCase):
-    """ProjectServiceOAuth2 unit test stubs"""
+class TestProjectServicePermission(unittest.TestCase):
+    """ProjectServicePermission unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectServiceOAuth2(self):
-        """Test ProjectServiceOAuth2"""
+    def testProjectServicePermission(self):
+        """Test ProjectServicePermission"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectServiceOAuth2()  # noqa: E501
+        # model = ProjectServicePermission()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_project_service_permission.py` & `ory-client-1.1.7/test/test_permissions_on_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_service_permission import ProjectServicePermission
+from ory_client.model.permissions_on_project import PermissionsOnProject
 
 
-class TestProjectServicePermission(unittest.TestCase):
-    """ProjectServicePermission unit test stubs"""
+class TestPermissionsOnProject(unittest.TestCase):
+    """PermissionsOnProject unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectServicePermission(self):
-        """Test ProjectServicePermission"""
+    def testPermissionsOnProject(self):
+        """Test PermissionsOnProject"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectServicePermission()  # noqa: E501
+        # model = PermissionsOnProject()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_project_services.py` & `ory-client-1.1.7/test/test_project_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_projects.py` & `ory-client-1.1.7/test/test_projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_quota_branding_themes.py` & `ory-client-1.1.7/test/test_quota_branding_themes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_recovery_code_for_identity.py` & `ory-client-1.1.7/test/test_recovery_code_for_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_recovery_flow.py` & `ory-client-1.1.7/test/test_recovery_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_recovery_flow_state.py` & `ory-client-1.1.7/test/test_recovery_flow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_recovery_identity_address.py` & `ory-client-1.1.7/test/test_recovery_identity_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_recovery_link_for_identity.py` & `ory-client-1.1.7/test/test_recovery_link_for_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_registration_flow.py` & `ory-client-1.1.7/test/test_registration_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_reject_o_auth2_request.py` & `ory-client-1.1.7/test/test_reject_o_auth2_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relation_query.py` & `ory-client-1.1.7/test/test_relation_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relationship.py` & `ory-client-1.1.7/test/test_relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relationship_api.py` & `ory-client-1.1.7/test/test_relationship_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relationship_namespaces.py` & `ory-client-1.1.7/test/test_relationship_namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relationship_patch.py` & `ory-client-1.1.7/test/test_relationship_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_relationships.py` & `ory-client-1.1.7/test/test_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_schema_patch.py` & `ory-client-1.1.7/test/test_identity_schema_preset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.schema_patch import SchemaPatch
+from ory_client.model.identity_schema_preset import IdentitySchemaPreset
 
 
-class TestSchemaPatch(unittest.TestCase):
-    """SchemaPatch unit test stubs"""
+class TestIdentitySchemaPreset(unittest.TestCase):
+    """IdentitySchemaPreset unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSchemaPatch(self):
-        """Test SchemaPatch"""
+    def testIdentitySchemaPreset(self):
+        """Test IdentitySchemaPreset"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SchemaPatch()  # noqa: E501
+        # model = IdentitySchemaPreset()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_self_service_flow_expired_error.py` & `ory-client-1.1.7/test/test_self_service_flow_expired_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_session.py` & `ory-client-1.1.7/test/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_session_authentication_method.py` & `ory-client-1.1.7/test/test_session_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_session_authentication_methods.py` & `ory-client-1.1.7/test/test_session_authentication_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_session_caching_quota.py` & `ory-client-1.1.7/test/test_session_caching_quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_session_device.py` & `ory-client-1.1.7/test/test_session_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_set_active_project_in_console_body.py` & `ory-client-1.1.7/test/test_set_active_project_in_console_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_set_custom_domain_body.py` & `ory-client-1.1.7/test/test_set_custom_domain_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_set_project.py` & `ory-client-1.1.7/test/test_set_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_set_project_branding_theme_body.py` & `ory-client-1.1.7/test/test_set_project_branding_theme_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_settings_flow.py` & `ory-client-1.1.7/test/test_settings_flow_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity import Identity
 from ory_client.model.settings_flow_state import SettingsFlowState
-from ory_client.model.ui_container import UiContainer
-globals()['Identity'] = Identity
-globals()['SettingsFlowState'] = SettingsFlowState
-globals()['UiContainer'] = UiContainer
-from ory_client.model.settings_flow import SettingsFlow
 
 
-class TestSettingsFlow(unittest.TestCase):
-    """SettingsFlow unit test stubs"""
+class TestSettingsFlowState(unittest.TestCase):
+    """SettingsFlowState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSettingsFlow(self):
-        """Test SettingsFlow"""
+    def testSettingsFlowState(self):
+        """Test SettingsFlowState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SettingsFlow()  # noqa: E501
+        # model = SettingsFlowState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_settings_flow_state.py` & `ory-client-1.1.7/test/test_verification_flow_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.settings_flow_state import SettingsFlowState
+from ory_client.model.verification_flow_state import VerificationFlowState
 
 
-class TestSettingsFlowState(unittest.TestCase):
-    """SettingsFlowState unit test stubs"""
+class TestVerificationFlowState(unittest.TestCase):
+    """VerificationFlowState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSettingsFlowState(self):
-        """Test SettingsFlowState"""
+    def testVerificationFlowState(self):
+        """Test VerificationFlowState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SettingsFlowState()  # noqa: E501
+        # model = VerificationFlowState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_source_position.py` & `ory-client-1.1.7/test/test_source_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_string_slice_json_format.py` & `ory-client-1.1.7/test/test_string_slice_json_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_stripe_customer.py` & `ory-client-1.1.7/test/test_stripe_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_subject_set.py` & `ory-client-1.1.7/test/test_subject_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_subscription.py` & `ory-client-1.1.7/test/test_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_successful_native_login.py` & `ory-client-1.1.7/test/test_successful_native_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_successful_native_registration.py` & `ory-client-1.1.7/test/test_successful_native_registration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_successful_project_update.py` & `ory-client-1.1.7/test/test_successful_project_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_token_pagination.py` & `ory-client-1.1.7/test/test_token_pagination_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.token_pagination import TokenPagination
+from ory_client.model.token_pagination_headers import TokenPaginationHeaders
 
 
-class TestTokenPagination(unittest.TestCase):
-    """TokenPagination unit test stubs"""
+class TestTokenPaginationHeaders(unittest.TestCase):
+    """TokenPaginationHeaders unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokenPagination(self):
-        """Test TokenPagination"""
+    def testTokenPaginationHeaders(self):
+        """Test TokenPaginationHeaders"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokenPagination()  # noqa: E501
+        # model = TokenPaginationHeaders()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_token_pagination_headers.py` & `ory-client-1.1.7/test/test_token_pagination_request_parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.token_pagination_headers import TokenPaginationHeaders
+from ory_client.model.token_pagination_request_parameters import TokenPaginationRequestParameters
 
 
-class TestTokenPaginationHeaders(unittest.TestCase):
-    """TokenPaginationHeaders unit test stubs"""
+class TestTokenPaginationRequestParameters(unittest.TestCase):
+    """TokenPaginationRequestParameters unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokenPaginationHeaders(self):
-        """Test TokenPaginationHeaders"""
+    def testTokenPaginationRequestParameters(self):
+        """Test TokenPaginationRequestParameters"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokenPaginationHeaders()  # noqa: E501
+        # model = TokenPaginationRequestParameters()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_token_pagination_request_parameters.py` & `ory-client-1.1.7/test/test_pagination.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.token_pagination_request_parameters import TokenPaginationRequestParameters
+from ory_client.model.pagination import Pagination
 
 
-class TestTokenPaginationRequestParameters(unittest.TestCase):
-    """TokenPaginationRequestParameters unit test stubs"""
+class TestPagination(unittest.TestCase):
+    """Pagination unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokenPaginationRequestParameters(self):
-        """Test TokenPaginationRequestParameters"""
+    def testPagination(self):
+        """Test Pagination"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokenPaginationRequestParameters()  # noqa: E501
+        # model = Pagination()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_token_pagination_response_headers.py` & `ory-client-1.1.7/test/test_token_pagination_response_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_trust_o_auth2_jwt_grant_issuer.py` & `ory-client-1.1.7/test/test_trust_o_auth2_jwt_grant_issuer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_issuer.py` & `ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_issuers.py` & `ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-client-1.1.7/test/test_trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_container.py` & `ory-client-1.1.7/test/test_ui_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node.py` & `ory-client-1.1.7/test/test_ui_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_anchor_attributes.py` & `ory-client-1.1.7/test/test_ui_node_anchor_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_attributes.py` & `ory-client-1.1.7/test/test_ui_node_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_image_attributes.py` & `ory-client-1.1.7/test/test_ui_node_image_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_input_attributes.py` & `ory-client-1.1.7/test/test_ui_node_input_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_meta.py` & `ory-client-1.1.7/test/test_ui_node_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_script_attributes.py` & `ory-client-1.1.7/test/test_ui_node_script_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_node_text_attributes.py` & `ory-client-1.1.7/test/test_ui_node_text_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_nodes.py` & `ory-client-1.1.7/test/test_ui_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_text.py` & `ory-client-1.1.7/test/test_ui_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_ui_texts.py` & `ory-client-1.1.7/test/test_ui_texts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_identity_body.py` & `ory-client-1.1.7/test/test_update_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_body.py` & `ory-client-1.1.7/test/test_update_login_flow_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_with_lookup_secret_method.py` & `ory-client-1.1.7/test/test_update_login_flow_with_lookup_secret_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_with_oidc_method.py` & `ory-client-1.1.7/test/test_update_login_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_with_password_method.py` & `ory-client-1.1.7/test/test_update_login_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_with_totp_method.py` & `ory-client-1.1.7/test/test_update_login_flow_with_totp_method.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_login_flow_with_web_authn_method.py` & `ory-client-1.1.7/test/test_update_login_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_recovery_flow_body.py` & `ory-client-1.1.7/test/test_update_recovery_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_recovery_flow_with_code_method.py` & `ory-client-1.1.7/test/test_update_recovery_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_recovery_flow_with_link_method.py` & `ory-client-1.1.7/test/test_update_recovery_flow_with_link_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_registration_flow_body.py` & `ory-client-1.1.7/test/test_update_registration_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_registration_flow_with_oidc_method.py` & `ory-client-1.1.7/test/test_update_registration_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_registration_flow_with_password_method.py` & `ory-client-1.1.7/test/test_update_registration_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_registration_flow_with_web_authn_method.py` & `ory-client-1.1.7/test/test_update_registration_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_body.py` & `ory-client-1.1.7/test/test_update_settings_flow_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_lookup_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_lookup_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_oidc_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_oidc_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_password_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_profile_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_profile_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_totp_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_totp_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_settings_flow_with_web_authn_method.py` & `ory-client-1.1.7/test/test_update_settings_flow_with_web_authn_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_subscription_body.py` & `ory-client-1.1.7/test/test_update_subscription_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_verification_flow_body.py` & `ory-client-1.1.7/test/test_update_verification_flow_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_verification_flow_with_code_method_body.py` & `ory-client-1.1.7/test/test_update_verification_flow_with_code_method_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_update_verification_flow_with_link_method.py` & `ory-client-1.1.7/test/test_update_verification_flow_with_link_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_verifiable_identity_address.py` & `ory-client-1.1.7/test/test_verifiable_identity_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_verification_flow.py` & `ory-client-1.1.7/test/test_verification_flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.1.5/test/test_verification_flow_state.py` & `ory-client-1.1.7/test/test_null_plan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.verification_flow_state import VerificationFlowState
+from ory_client.model.null_plan import NullPlan
 
 
-class TestVerificationFlowState(unittest.TestCase):
-    """VerificationFlowState unit test stubs"""
+class TestNullPlan(unittest.TestCase):
+    """NullPlan unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVerificationFlowState(self):
-        """Test VerificationFlowState"""
+    def testNullPlan(self):
+        """Test NullPlan"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = VerificationFlowState()  # noqa: E501
+        # model = NullPlan()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_version.py` & `ory-client-1.1.7/test/test_warning.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.version import Version
+from ory_client.model.warning import Warning
 
 
-class TestVersion(unittest.TestCase):
-    """Version unit test stubs"""
+class TestWarning(unittest.TestCase):
+    """Warning unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVersion(self):
-        """Test Version"""
+    def testWarning(self):
+        """Test Warning"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Version()  # noqa: E501
+        # model = Warning()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.1.5/test/test_wellknown_api.py` & `ory-client-1.1.7/test/test_wellknown_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.1.5
+    The version of the OpenAPI document: v1.1.7
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

